<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Global Logistics Expert Dashboard - 2026 Jan</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <script src="https://cdnjs.cloudflare.com/ajax/libs/html2pdf.js/0.10.1/html2pdf.bundle.min.js" crossorigin="anonymous"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap');
        
        * { box-sizing: border-box; } /* 모든 요소 박스 모델 고정 */
        
        body { font-family: 'Inter', sans-serif; background-color: #f8fafc; margin: 0; }
        .card-shadow { box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1); }
        
        /* [최적화] 상태 배지 및 텍스트 줄바꿈 방지 */
        .status-pill { 
            display: inline-block;
            padding: 4px 12px; 
            border-radius: 9999px; 
            font-size: 0.75rem; 
            font-weight: 700; 
            white-space: nowrap; 
        }
        .nowrap-text { white-space: nowrap; }

        .detail-row { display: none; background-color: #fefce8; }
        .detail-row.active { display: table-row; }
        
        /* [최적화] 테이블 레이아웃 엄격 고정 */
        .table-fixed-layout { 
            table-layout: fixed; 
            min-width: 800px; /* 가로 스크롤 유발 최소 너비 */
            width: 100%; 
            border-collapse: collapse;
        }

        /* 각 컬럼 너비 강제 할당 */
        .col-route { width: 30%; }
        .col-status { width: 20%; }
        .col-lt { width: 25%; }
        .col-insight { width: 25%; }

        /* [최적화] 텍스트가 박스를 벗어나지 않도록 처리 */
        .truncate-custom {
            overflow: hidden;
            text-overflow: ellipsis;
            white-space: nowrap;
            display: block;
            width: 100%;
        }

        .break-words-custom {
            word-break: break-all;
            word-wrap: break-word;
            white-space: normal;
        }

        #toast { visibility: hidden; min-width: 250px; background-color: #1e293b; color: #fff; text-align: center; border-radius: 8px; padding: 16px; position: fixed; z-index: 1000; left: 50%; bottom: 30px; transform: translateX(-50%); }
        #toast.show { visibility: visible; animation: fadein 0.5s, fadeout 0.5s 2.5s; }
        @keyframes fadein { from {bottom: 0; opacity: 0;} to {bottom: 30px; opacity: 1;} }
        @keyframes fadeout { from {bottom: 30px; opacity: 1;} to {bottom: 0; opacity: 0;} }

        /* 가로 스크롤바 커스텀 */
        .overflow-x-auto::-webkit-scrollbar { height: 8px; }
        .overflow-x-auto::-webkit-scrollbar-track { background: #f1f5f9; }
        .overflow-x-auto::-webkit-scrollbar-thumb { background: #cbd5e1; border-radius: 10px; }
    </style>
</head>
<body>

    <main id="reportContent" class="p-4 md:p-12 max-w-7xl mx-auto">
        
        <!-- Header -->
        <header class="flex flex-col md:flex-row justify-between items-start md:items-center mb-10 gap-4">
            <div>
                <div class="flex items-center gap-3 mb-2">
                    <span class="bg-amber-400 text-slate-900 px-3 py-1 rounded-md text-xs font-bold uppercase tracking-wider">Logistics Expert Insight</span>
                    <span class="text-slate-400 text-xs">2026.01 Monthly Analysis</span>
                </div>
                <h2 class="text-3xl font-bold text-slate-800">2026년 1월 글로벌 해운 물류 시황 심층 분석</h2>
                <p class="text-red-600 font-bold mt-1 leading-tight">실무 긴급: 춘절(LNY) 'Red Zone' 진입 및 호주/북미 공급망 위기 대응</p>
            </div>
            <div class="flex space-x-2 print:hidden shrink-0">
                <button onclick="downloadHTML()" class="bg-amber-400 text-slate-900 px-5 py-2.5 rounded-lg text-sm font-bold hover:bg-amber-500 transition-all shadow-lg shadow-amber-200/50">
                    <i class="fas fa-file-code mr-2"></i> 대시보드 파일 추출
                </button>
                <button onclick="downloadPDF()" class="bg-white border border-slate-200 px-5 py-2.5 rounded-lg text-sm font-medium hover:bg-slate-50 transition-all">
                    <i class="fas fa-file-pdf mr-2 text-red-500"></i> PDF 저장
                </button>
            </div>
        </header>

        <!-- Summary section (Omitted for brevity, keeping the same structure as previous) -->
        <section id="summary" class="mb-12">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-8">
                <div class="lg:col-span-7 bg-white p-8 rounded-2xl card-shadow border border-slate-100">
                    <h3 class="text-xl font-bold text-slate-800 mb-8 flex items-center">
                        <span class="w-2 h-7 bg-red-600 mr-4 rounded-full"></span>
                        AI 총평: 수출 담당자 즉시 대응 가이드
                    </h3>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                        <div class="p-5 bg-red-50 rounded-2xl border border-red-100">
                            <p class="text-sm font-bold text-red-800 mb-3 flex items-center"><i class="fas fa-clock mr-2"></i> [최우선] 춘절(LNY) Red Zone</p>
                            <p class="text-xs text-red-700 leading-relaxed font-medium break-words-custom">1/20~1/26이 선적 골든타임입니다. 이후 선복 마감 및 프리미엄 운임(GRI) 요구가 확실시됩니다.</p>
                        </div>
                        <div class="p-5 bg-amber-50 rounded-2xl border border-amber-100">
                            <p class="text-sm font-bold text-amber-800 mb-3 flex items-center"><i class="fas fa-exclamation-triangle mr-2"></i> [위험] 호주 항만 파업 지속</p>
                            <p class="text-xs text-amber-700 leading-relaxed font-medium break-words-custom">DP World 파업으로 MEL/AKL 리드타임 +7일 이상 발생. 시드니 양하 대안을 검토하십시오.</p>
                        </div>
                        <div class="p-5 bg-slate-50 rounded-2xl border border-slate-100">
                            <p class="text-sm font-bold text-slate-800 mb-3 flex items-center"><i class="fas fa-snowflake mr-2"></i> 북미/북유럽 혹한기 병목</p>
                            <p class="text-xs text-slate-600 leading-relaxed font-medium break-words-custom">밴쿠버 철송 체류 7.7일. 내륙 LT에 7~10일의 'Winter Buffer'를 설정하십시오.</p>
                        </div>
                        <div class="p-5 bg-slate-50 rounded-2xl border border-slate-100">
                            <p class="text-sm font-bold text-slate-800 mb-3 flex items-center"><i class="fas fa-shield-alt mr-2"></i> CIS 제재 및 구조적 변화</p>
                            <p class="text-xs text-slate-600 leading-relaxed font-medium break-words-custom">러시아향 전략물자 통제 강화. 중앙아시아는 Middle Corridor 대안을 고려하십시오.</p>
                        </div>
                    </div>
                </div>
                <div class="lg:col-span-5 bg-slate-900 text-white p-8 rounded-2xl card-shadow flex flex-col justify-center">
                    <h3 class="text-xl font-bold mb-8 flex justify-between items-center">
                        <span class="leading-tight">[Action Priority]<br>Global Risk Heatmap</span>
                        <span class="text-[10px] bg-red-600 px-2 py-1 rounded font-bold uppercase tracking-widest">Weight x1.5</span>
                    </h3>
                    <div class="space-y-8">
                        <div>
                            <div class="flex justify-between text-xs mb-3">
                                <span class="text-red-400 font-bold uppercase tracking-wide">춘절 전 선복 고갈</span>
                                <span class="text-red-400 font-bold">98% Critical</span>
                            </div>
                            <div class="w-full bg-slate-800 h-2.5 rounded-full overflow-hidden">
                                <div class="bg-gradient-to-r from-red-600 to-orange-500 h-full w-[98%]"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between text-xs mb-3">
                                <span class="text-amber-400 font-bold uppercase tracking-wide">호주 항만 파업</span>
                                <span class="text-amber-400 font-bold">90% High</span>
                            </div>
                            <div class="w-full bg-slate-800 h-2.5 rounded-full overflow-hidden">
                                <div class="bg-gradient-to-r from-amber-500 to-amber-300 h-full w-[90%]"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between text-xs mb-3">
                                <span class="text-slate-300 uppercase tracking-wide">GSCPI 공급망 압력</span>
                                <span class="text-slate-300 font-bold">85% High</span>
                            </div>
                            <div class="w-full bg-slate-800 h-2.5 rounded-full overflow-hidden">
                                <div class="bg-slate-500 h-full w-[85%]"></div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Metrics section (Keeping values same) -->
        <section id="metrics" class="mb-12">
            <h3 class="text-sm font-bold text-slate-400 mb-6 uppercase tracking-[0.2em]">핵심 물류 시장 지표</h3>
            <div class="grid grid-cols-2 md:grid-cols-5 gap-6">
                <div class="bg-white p-6 rounded-2xl card-shadow border border-slate-100">
                    <p class="text-xs text-slate-400 font-bold mb-2">SCFI (운임지수)</p>
                    <div class="flex items-end justify-between">
                        <span class="text-2xl font-bold text-slate-800">1,574.12</span>
                        <span class="text-red-500 text-xs font-bold bg-red-50 px-1.5 py-0.5 rounded">↑ 1.37%</span>
                    </div>
                </div>
                <div class="bg-white p-6 rounded-2xl card-shadow border border-slate-100">
                    <p class="text-xs text-slate-400 font-bold mb-2">GSCPI (압력)</p>
                    <div class="flex items-end justify-between">
                        <span class="text-2xl font-bold text-slate-800">0.51</span>
                        <span class="text-red-500 text-xs font-bold uppercase">Rising</span>
                    </div>
                </div>
                <div class="bg-white p-6 rounded-2xl card-shadow border border-slate-100">
                    <p class="text-xs text-slate-400 font-bold mb-2">WTI (유가)</p>
                    <div class="flex items-end justify-between">
                        <span class="text-2xl font-bold text-slate-800">$59.41</span>
                        <span class="text-red-500 text-xs font-bold bg-red-50 px-1.5 py-0.5 rounded">↑ 2.41%</span>
                    </div>
                </div>
                <div class="bg-white p-6 rounded-2xl card-shadow border border-slate-100">
                    <p class="text-xs text-slate-400 font-bold mb-2">BAF (벙커가)</p>
                    <div class="flex items-end justify-between">
                        <span class="text-2xl font-bold text-slate-800">~$758</span>
                        <span class="text-red-500 text-xs font-bold uppercase">High</span>
                    </div>
                </div>
                <div class="bg-white p-6 rounded-2xl card-shadow border border-slate-100">
                    <p class="text-xs text-slate-400 font-bold mb-2">ERAI (철송)</p>
                    <div class="flex items-end justify-between">
                        <span class="text-2xl font-bold text-slate-800">Stable</span>
                        <span class="text-slate-400 text-xs">-</span>
                    </div>
                </div>
            </div>
        </section>

        <!-- Route Status Table (Enhanced) -->
        <section id="regional" class="mb-12">
            <div class="flex flex-col md:flex-row justify-between items-start md:items-center mb-8 gap-6">
                <h3 class="text-xl font-bold text-slate-800 uppercase tracking-wide">부산항 발 33개 운영 루트 상세 현황</h3>
                <div class="flex flex-wrap gap-3 print:hidden">
                    <div class="relative">
                        <i class="fas fa-search absolute left-3 top-3 text-slate-300 text-sm"></i>
                        <input type="text" id="portSearch" placeholder="항만 또는 국가 검색..." class="pl-10 pr-4 py-2.5 border border-slate-200 rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-amber-400 w-64 transition-all">
                    </div>
                    <select id="regionFilter" class="px-4 py-2.5 border border-slate-200 rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-amber-400 bg-white">
                        <option value="all">전체 권역 보기</option>
                        <option value="sea">동남아/서남아</option>
                        <option value="oceania">오세아니아</option>
                        <option value="na">북미/남미</option>
                        <option value="ea">동아시아</option>
                        <option value="eu">유럽/지중해</option>
                        <option value="cis">러시아/CIS</option>
                    </select>
                </div>
            </div>

            <div class="bg-white rounded-3xl card-shadow border border-slate-100 overflow-hidden">
                <div class="overflow-x-auto">
                    <!-- [핵심] table-layout: fixed 및 최소 너비 강제 -->
                    <table class="table-fixed-layout">
                        <thead class="bg-slate-50 border-b border-slate-200">
                            <tr>
                                <th class="col-route px-8 py-5 text-xs font-bold text-slate-500 uppercase tracking-wider text-left">Route (Port)</th>
                                <th class="col-status px-8 py-5 text-xs font-bold text-slate-500 uppercase tracking-wider text-left">Status</th>
                                <th class="col-lt px-8 py-5 text-xs font-bold text-slate-500 uppercase tracking-wider text-left">Lead Time</th>
                                <th class="col-insight px-8 py-5 text-xs font-bold text-slate-500 uppercase tracking-wider text-center">Insights</th>
                            </tr>
                        </thead>
                        <tbody id="portTableBody" class="divide-y divide-slate-100">
                            <!-- JS에 의해 렌더링 -->
                        </tbody>
                    </table>
                </div>
            </div>
        </section>

        <footer class="mb-20 py-10 text-center border-t border-slate-100">
            <p class="text-slate-400 text-xs font-medium">© 2026 Logistics Strategic Analysis Center. 모든 데이터는 부산항(Busan) 출발 기준입니다.</p>
        </footer>

    </main>

    <div id="toast">파일이 추출되었습니다.</div>

    <script>
        const portData = [
            // 동남아/서남아
            { id: "p1", name: "Port Kelang", country: "Malaysia", region: "sea", status: "Caution", lt: "10-14일", detail: "춘절 전 물량 집중으로 선복 확보가 어렵습니다. 포트 클랑은 환적 허브로서 야드 밀도가 높으나, 터미널 운영은 비교적 안정적입니다." },
            { id: "p2", name: "MANILA", country: "Philippines", region: "sea", status: "Normal", lt: "5-9일", detail: "마닐라 북항과 남항 모두 운영이 원활합니다. 통관 강화 이슈가 발생할 수 있으니 서류 준비에 만전을 기하십시오." },
            { id: "p3", name: "BANGKOK", country: "Thailand", region: "sea", status: "Caution", lt: "12-16일", detail: "방콕항은 주로 람차방을 경유합니다. 현재 람차방의 환적 물량 증가로 바지선 연결이 지연될 수 있습니다." },
            { id: "p4", name: "SIHANOUKVILLE", country: "Cambodia", region: "sea", status: "Caution", lt: "14-18일", detail: "환적 서비스 위주 운영. 환적항에서의 연결 지연 리스크를 고려하십시오." },
            { id: "p5", name: "JAKARTA", country: "Indonesia", region: "sea", status: "Caution", lt: "10-15일", detail: "자카르타 탄중 프리옥 혼잡도 상승. 세관 'Red Line' 검사 비율이 높아지는 시기입니다." },
            { id: "p6", name: "SINGAPORE", country: "Singapore", region: "sea", status: "Normal", lt: "7-10일", detail: "세계 최대 허브로서 효율 유지 중. 춘절 전 환적 화물 폭증으로 야드 적체율은 높은 편입니다." },

            // 오세아니아
            { id: "p7", name: "MELBOURNE", country: "Australia", region: "oceania", status: "Critical", lt: "18-28일(+)", detail: "DP World 파업으로 선박 체선 심각. 선사들이 기항을 건너뛰는 경우가 빈번하므로 실시간 스케줄 확인 필수." },
            { id: "p8", name: "AUCKLAND", country: "New Zealand", region: "oceania", status: "Caution", lt: "20-30일", detail: "호주 항만 파업 여파가 오클랜드 향 서비스 지연으로 직결됩니다. 직항 서비스 위주로 확보하십시오." },

            // 북미/남미
            { id: "p9", name: "VANCOUVER", country: "Canada", region: "na", status: "Caution", lt: "14-20일", detail: "터미널 내 철도 조차장 혼잡. 로컬 화물이라도 터미널 반출 속도가 느려질 수 있습니다." },
            { id: "p10", name: "MISSISSAUGA (Rail)", country: "Canada (Toronto)", region: "na", status: "Critical", lt: "35-50일", detail: "밴쿠버발 철송 지연(평균 7.7일)과 혹한으로 인한 철도 운행 속도 저하가 심각합니다." },
            { id: "p11", name: "MISSISSAUGA (Truck)", country: "Canada (Vancouver)", region: "na", status: "Critical", lt: "25-35일", detail: "로키 산맥 기상 악화로 도로 폐쇄 위험 높음. 비용이 상승 중이나 철송보다는 빠를 수 있습니다." },
            { id: "p12", name: "SEATTLE", country: "USA", region: "na", status: "Normal", lt: "12-16일", detail: "캘리포니아 대비 혼잡도 낮고 원활. 미 중서부 내륙 화물 진입점으로 강력 추천됩니다." },
            { id: "p13", name: "LONG BEACH", country: "USA", region: "na", status: "Caution", lt: "12-18일", detail: "레일카 부족으로 컨테이너 터미널 체류 5~7일 증가. 사전 배차 계획이 필요합니다." },
            { id: "p14", name: "NEW YORK", country: "USA", region: "na", status: "Caution", lt: "28-40일", detail: "파나마 운하 제한 및 희망봉 우회 고착화로 선박별 LT 편차가 극심합니다." },
            { id: "p15", name: "SAVANNAH", country: "USA", region: "na", status: "Caution", lt: "30-38일", detail: "희망봉 우회 선박들이 일시에 몰리는 Vessel Bunching 현상으로 하역 지연 리스크가 있습니다." },
            { id: "p16", name: "VITORIA", country: "Brazil", region: "na", status: "Normal", lt: "35-45일", detail: "브라질 주요 항만 중 산토스 대비 혼잡도 낮음. 부산발 직항 서비스 드문 편입니다." },

            // 동아시아
            { id: "p17", name: "KAOHSIUNG", country: "Taiwan", region: "ea", status: "Normal", lt: "3-5일", detail: "대만 주요 환적항으로 운영 안정적. 부산발 서비스 빈도 높아 선복 확보 용이." },
            { id: "p18", name: "KEELUNG", country: "Taiwan", region: "ea", status: "Normal", lt: "3-5일", detail: "원활한 흐름 유지 중. 특이사항 없음." },
            { id: "p19", name: "HONG KONG", country: "Hong Kong", region: "ea", status: "Normal", lt: "3-5일", detail: "춘절 전 중국 주강삼각주 바지선 피더 네트워크 지연 리스크가 존재합니다." },
            { id: "p20", name: "YOKOHAMA", country: "Japan", region: "ea", status: "Normal", lt: "2-4일", detail: "매우 안정적. 한-일 노선 선복 공급 원활." },
            { id: "p21", name: "HAKATA", country: "Japan", region: "ea", status: "Normal", lt: "1-2일", detail: "부산과 가장 가까운 항만. 페리 이용 시 당일/익일 통관 가능하여 긴급 화물에 최적." },

            // 유럽/지중해
            { id: "p22", name: "SOUTHAMPTON", country: "UK", region: "eu", status: "Caution", lt: "40-50일", detail: "희망봉 우회로 LT 장기화. 겨울철 강풍 등 기상 악화 시 항만 운영 일시 중단 주의." },
            { id: "p23", name: "ROTTERDAM", country: "Netherlands", region: "eu", status: "Caution", lt: "38-48일", detail: "겨울 폭풍 여파로 터미널 효율 저하. 바지선 연결 지연이 불가피합니다." },
            { id: "p24", name: "ISTANBUL", country: "Turkey", region: "eu", status: "Normal", lt: "35-45일", detail: "암바리 항만 큰 혼잡 없음. Middle Corridor 활성화로 가치 상승 중." },

            // 러시아/CIS
            { id: "p25", name: "TOSHKENT", country: "Uzbekistan", region: "cis", status: "Caution", lt: "30-45일", detail: "중국 경유 TCR 루트. 중국-카자흐 국경 화차 교환 병목으로 국경 통과 7~10일 소요." },
            { id: "p26", name: "BISHKEK (TCR)", country: "Kyrgyzstan", region: "cis", status: "Caution", lt: "35-50일", detail: "폭설 시 산악 국경 폐쇄 빈번. 동절기 추가 리드타임 확보 필수." },
            { id: "p27", name: "VLADIVOSTOK", country: "Russia", region: "cis", status: "Caution", lt: "2-5일", detail: "제재 준수(HS Code 체크) 필수. 전략물자 통제로 서류 심사가 매우 까다롭습니다." },
            { id: "p28", name: "MOSCOW (TSR)", country: "Russia", region: "cis", status: "Critical", lt: "25-35일", detail: "RZD 화차 부족 및 군수 물자 우선 배정으로 민간 화물 스케줄 불안정." },
            { id: "p29", name: "NOVOSIBIRSK (TSR)", country: "Russia", region: "cis", status: "Critical", lt: "20-30일", detail: "혹한기(-40도) 장비 고장으로 인한 철송 지연 및 속도 제한 상시 발생." },
            { id: "p30", name: "MOSCOW (Truck)", country: "Russia", region: "cis", status: "Critical", lt: "18-25일", detail: "철송 대안이나 결빙 도로 리스크 및 운전자 부족 문제로 긴급 화물에만 한정 사용." },
            { id: "p31", name: "NOVOSIBIRSK (Truck)", country: "Russia", region: "cis", status: "Critical", lt: "12-18일", detail: "장거리 운송 리스크 상존. 동결 방지 위해 보온/냉장 트럭 사용 권장." },
            { id: "p32", name: "ALMATY (TCR)", country: "Kazakhstan", region: "cis", status: "Caution", lt: "25-35일", detail: "중앙아시아 물류 허브. 춘절 전 국경 혼잡 가중 예상되나 TCR 수혜로 사정 양호." },
            { id: "p33", name: "ULAANBAATAR", country: "Mongolia", region: "cis", status: "Caution", lt: "15-25일", detail: "중국 톈진항 적체 및 얼리안 국경 환적 지연 리스크 상시 체크." }
        ];

        function renderTable(data) {
            const body = document.getElementById('portTableBody');
            body.innerHTML = '';
            data.forEach(port => {
                const tr = document.createElement('tr');
                tr.className = "hover:bg-slate-50 transition-colors cursor-pointer group";
                tr.onclick = () => toggleDetail(port.id);
                
                let statusClass = "bg-green-100 text-green-700";
                if(port.status === "Caution") statusClass = "bg-amber-100 text-amber-700";
                if(port.status === "Critical") statusClass = "bg-red-100 text-red-700";

                tr.innerHTML = `
                    <td class="px-8 py-5 col-route">
                        <div class="font-bold text-slate-800 leading-tight truncate-custom" title="${port.name}">${port.name}</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase tracking-wider truncate-custom">${port.country}</div>
                    </td>
                    <td class="px-8 py-5 col-status">
                        <span class="status-pill ${statusClass}">${port.status}</span>
                    </td>
                    <td class="px-8 py-5 col-lt">
                        <span class="text-sm text-slate-600 font-semibold nowrap-text">${port.lt}</span>
                    </td>
                    <td class="px-8 py-5 col-insight text-center">
                        <i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500 transition-all"></i>
                    </td>
                `;
                
                const detailTr = document.createElement('tr');
                detailTr.id = `detail-${port.id}`;
                detailTr.className = "detail-row";
                detailTr.innerHTML = `
                    <td colspan="4" class="px-12 py-6">
                        <div class="flex items-start">
                            <div class="w-10 h-10 bg-amber-100 rounded-2xl flex items-center justify-center mr-5 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600"></i>
                            </div>
                            <div class="flex-1 break-words-custom">
                                <p class="text-xs font-bold text-amber-800 uppercase mb-1">Expert Deep Insight</p>
                                <p class="text-sm text-slate-700 leading-relaxed font-medium">${port.detail}</p>
                            </div>
                        </div>
                    </td>
                `;
                body.appendChild(tr);
                body.appendChild(detailTr);
            });
        }

        function toggleDetail(id) {
            const row = document.getElementById(`detail-${id}`);
            if (!row) return;
            const isActive = row.classList.contains('active');
            if(isActive) {
                row.classList.remove('active');
            } else {
                row.classList.add('active');
            }
        }

        function filterData() {
            const search = document.getElementById('portSearch').value.toLowerCase();
            const region = document.getElementById('regionFilter').value;
            const filtered = portData.filter(p => {
                const matchesSearch = p.name.toLowerCase().includes(search) || p.country.toLowerCase().includes(search);
                const matchesRegion = region === 'all' || p.region === region;
                return matchesSearch && matchesRegion;
            });
            renderTable(filtered);
        }

        function downloadHTML() {
            const blob = new Blob([document.documentElement.outerHTML], { type: 'text/html' });
            const url = URL.createObjectURL(blob);
            const a = document.createElement('a');
            a.href = url;
            a.download = 'Logistics_Expert_Dashboard_Jan2026.html';
            a.click();
            URL.revokeObjectURL(url);
            showToast();
        }

        async function downloadPDF() {
            const opt = { 
                margin: 10, 
                filename: 'Logistics_Expert_Dashboard_Jan2026.pdf', 
                image: { type: 'jpeg', quality: 0.98 }, 
                html2canvas: { scale: 2 }, 
                jsPDF: { unit: 'mm', format: 'a4', orientation: 'portrait' } 
            };
            await html2pdf().set(opt).from(document.getElementById('reportContent')).save();
        }

        function showToast() {
            const t = document.getElementById("toast");
            t.className = "show";
            setTimeout(() => { t.className = t.className.replace("show", ""); }, 3000);
        }

        document.getElementById('portSearch').addEventListener('input', filterData);
        document.getElementById('regionFilter').addEventListener('change', filterData);
        window.onload = () => renderTable(portData);
    </script>

</body>
</html>
