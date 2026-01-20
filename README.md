<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>2026 Jan Global Logistics Dashboard</title>
    <!-- Tailwind CSS & Font Awesome -->
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <!-- html2pdf.js for PDF export -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/html2pdf.js/0.10.1/html2pdf.bundle.min.js"></script>
    
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Pretendard:wght@400;600;700&display=swap');
        
        body { 
            font-family: 'Pretendard', sans-serif; 
            background-color: #f1f5f9; 
            color: #1e293b;
        }

        .card-shadow { 
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.05), 0 4px 6px -2px rgba(0, 0, 0, 0.05); 
        }

        .status-pill { 
            padding: 4px 12px; 
            border-radius: 9999px; 
            font-size: 0.75rem; 
            font-weight: 700; 
            /* 가이드라인 준수: 줄바꿈 방지 */
            white-space: nowrap; 
        }

        /* 가이드라인 준수: 고정 컬럼 너비 및 최소 너비 설정 */
        .table-container {
            overflow-x: auto; /* 반응형 가로 스크롤 */
            border-radius: 1rem;
        }

        .custom-table {
            table-layout: fixed; /* 너비 고정 */
            min-width: 800px;    /* 최소 너비 보장 */
            width: 100%;
        }

        /* 컬럼별 비율 할당 */
        .col-route { width: 30%; }
        .col-status { width: 15%; }
        .col-lt { width: 20%; }
        .col-insight { width: 35%; }

        .detail-row { 
            display: none; 
            background-color: #fffbeb; 
        }
        .detail-row.active { 
            display: table-row; 
        }

        /* 유틸리티 */
        .nowrap { white-space: nowrap; }
    </style>
</head>
<body class="p-4 md:p-8">

    <div id="captureArea" class="max-w-7xl mx-auto space-y-8">
        
        <!-- Header Section -->
        <header class="flex flex-col md:flex-row justify-between items-start md:items-center gap-6">
            <div>
                <div class="flex items-center gap-2 mb-2">
                    <span class="bg-indigo-600 text-white px-3 py-1 rounded text-[10px] font-bold tracking-widest uppercase">Expert Analysis</span>
                    <span class="text-slate-400 text-xs">Updated: 2026.01.20</span>
                </div>
                <h1 class="text-2xl md:text-3xl font-bold text-slate-900 leading-tight">
                    2026년 1월 글로벌 해운 물류 시황 심층 분석
                </h1>
                <p class="text-red-500 font-bold mt-1 text-sm">
                    <i class="fas fa-exclamation-circle mr-1"></i> 긴급: 춘절 전 'Red Zone' 진입 및 공급망 리스크 대응 필요
                </p>
            </div>
            
            <div class="flex gap-3 print:hidden">
                <!-- HTML 저장 버튼 추가 -->
                <button onclick="exportToHTML()" class="flex items-center gap-2 px-5 py-2.5 bg-indigo-600 text-white rounded-xl text-sm font-semibold hover:bg-indigo-700 transition-all card-shadow">
                    <i class="fas fa-code"></i> HTML 추출
                </button>
                <button onclick="exportToPDF()" class="flex items-center gap-2 px-5 py-2.5 bg-white border border-slate-200 rounded-xl text-sm font-semibold hover:bg-slate-50 transition-all card-shadow">
                    <i class="fas fa-file-pdf text-red-500"></i> PDF 저장
                </button>
            </div>
        </header>

        <!-- AI Summary & Priorities -->
        <section class="grid grid-cols-1 lg:grid-cols-3 gap-6">
            <div class="lg:col-span-2 bg-white p-6 rounded-2xl card-shadow border border-slate-100">
                <h3 class="text-lg font-bold mb-6 flex items-center">
                    <span class="w-1.5 h-6 bg-indigo-600 mr-3 rounded-full"></span>
                    수출 담당자 핵심 실행 가이드
                </h3>
                <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                    <div class="p-4 bg-red-50 rounded-xl border border-red-100">
                        <h4 class="text-sm font-bold text-red-800 mb-2 flex items-center">
                            <i class="fas fa-calendar-alt mr-2"></i> [Critical] 춘절 대비 즉시 부킹
                        </h4>
                        <p class="text-xs text-red-700 leading-relaxed">
                            1/20~1/26 사이가 골든타임입니다. 이후 선복 마감 및 프리미엄 운임(GRI)이 확실시되니 2월 물량까지 선점하십시오.
                        </p>
                    </div>
                    <div class="p-4 bg-amber-50 rounded-xl border border-amber-100">
                        <h4 class="text-sm font-bold text-amber-800 mb-2 flex items-center">
                            <i class="fas fa-anchor mr-2"></i> [High] 호주 항만 파업 위기
                        </h4>
                        <p class="text-xs text-amber-700 leading-relaxed">
                            MEL/AKL 루트 리드타임 +7일 발생. 시드니 양하 후 내륙 운송 대안이나 파업 영향이 적은 터미널 이용을 검토하십시오.
                        </p>
                    </div>
                    <div class="p-4 bg-slate-50 rounded-xl border border-slate-200">
                        <h4 class="text-sm font-bold text-slate-800 mb-2 flex items-center">
                            <i class="fas fa-snowflake mr-2"></i> [Med-High] 북미/유럽 혹한 병목
                        </h4>
                        <p class="text-xs text-slate-600 leading-relaxed">
                            캐나다 철송 체류 평균 7.7일. 북유럽 겨울 폭풍으로 야적장 밀도 상승. 내륙 운송에 10일 이상의 버퍼를 설정하십시오.
                        </p>
                    </div>
                    <div class="p-4 bg-slate-50 rounded-xl border border-slate-200">
                        <h4 class="text-sm font-bold text-slate-800 mb-2 flex items-center">
                            <i class="fas fa-shield-alt mr-2"></i> [Medium] CIS 제재 준수
                        </h4>
                        <p class="text-xs text-slate-600 leading-relaxed">
                            러시아향 전략물자 통제 강화. 선적 전 Compliance 체크 필수. 중앙아시아는 Middle Corridor 대안을 우선 고려하십시오.
                        </p>
                    </div>
                </div>
            </div>
            
            <!-- Market Heatmap Metrics -->
            <div class="bg-slate-900 text-white p-6 rounded-2xl card-shadow flex flex-col justify-between">
                <div>
                    <h3 class="text-lg font-bold mb-1">Global Market Indices</h3>
                    <p class="text-slate-400 text-xs mb-6">2026.01 월간 주요 지표 요약</p>
                    
                    <div class="space-y-4">
                        <div class="flex justify-between items-center">
                            <span class="text-sm text-slate-400">SCFI (운임)</span>
                            <div class="text-right">
                                <div class="font-bold">1,574.12</div>
                                <div class="text-[10px] text-red-400"><i class="fas fa-caret-up"></i> 1.37%</div>
                            </div>
                        </div>
                        <div class="flex justify-between items-center">
                            <span class="text-sm text-slate-400">GSCPI (압력지수)</span>
                            <div class="text-right">
                                <div class="font-bold">0.51</div>
                                <div class="text-[10px] text-red-400">급등 (긴장 구간)</div>
                            </div>
                        </div>
                        <div class="flex justify-between items-center">
                            <span class="text-sm text-slate-400">WTI (유가)</span>
                            <div class="text-right">
                                <div class="font-bold">$59.41</div>
                                <div class="text-[10px] text-red-400"><i class="fas fa-caret-up"></i> 2.41%</div>
                            </div>
                        </div>
                        <div class="flex justify-between items-center">
                            <span class="text-sm text-slate-400">BAF (벙커료)</span>
                            <div class="text-right">
                                <div class="font-bold">~$758 / 톤</div>
                                <div class="text-[10px] text-amber-400">상승 추세</div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="mt-6 pt-4 border-t border-slate-800">
                    <p class="text-[10px] text-slate-500 leading-relaxed">
                        * GSCPI의 급등은 글로벌 물류 병목의 재시작을 의미하며 정시성 하락을 예고합니다.
                    </p>
                </div>
            </div>
        </section>

        <!-- Route Status Section -->
        <section class="space-y-4">
            <div class="flex flex-col md:flex-row justify-between items-start md:items-end gap-4">
                <h3 class="text-xl font-bold text-slate-900">부산항 발 33개 운영 루트 실시간 현황</h3>
                <div class="flex gap-2 w-full md:w-auto">
                    <div class="relative flex-1 md:w-64">
                        <i class="fas fa-search absolute left-3 top-3 text-slate-400 text-sm"></i>
                        <input type="text" id="routeSearch" placeholder="항만 또는 국가 검색..." class="w-full pl-10 pr-4 py-2 border border-slate-200 rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-indigo-500 transition-all">
                    </div>
                    <select id="regionFilter" class="px-4 py-2 border border-slate-200 rounded-xl text-sm bg-white focus:outline-none focus:ring-2 focus:ring-indigo-500">
                        <option value="all">전체 권역</option>
                        <option value="sea">동남아/서남아</option>
                        <option value="oceania">오세아니아</option>
                        <option value="na">북미/남미</option>
                        <option value="ea">동아시아</option>
                        <option value="eu">유럽/지중해</option>
                        <option value="cis">러시아/CIS</option>
                    </select>
                </div>
            </div>

            <div class="table-container bg-white card-shadow border border-slate-100">
                <table class="custom-table" id="routeTable">
                    <thead class="bg-slate-50 border-b border-slate-200">
                        <tr>
                            <th class="col-route px-6 py-4 text-left text-xs font-bold text-slate-500 uppercase tracking-wider">노선명 (Route)</th>
                            <th class="col-status px-6 py-4 text-left text-xs font-bold text-slate-500 uppercase tracking-wider">상태</th>
                            <th class="col-lt px-6 py-4 text-left text-xs font-bold text-slate-500 uppercase tracking-wider">예상 리드타임</th>
                            <th class="col-insight px-6 py-4 text-left text-xs font-bold text-slate-500 uppercase tracking-wider">Expert Insight (클릭)</th>
                        </tr>
                    </thead>
                    <tbody id="routeTableBody" class="divide-y divide-slate-100 font-medium">
                        <!-- Dynamic Rows -->
                    </tbody>
                </table>
            </div>
        </section>

        <footer class="text-center py-12 border-t border-slate-200">
            <p class="text-slate-400 text-xs">© 2026 Global Logistics Analysis Team. All data based on Busan Port Departures.</p>
        </footer>
    </div>

    <!-- Toast Message -->
    <div id="toast" class="fixed bottom-8 left-1/2 -translate-x-1/2 px-6 py-3 bg-slate-800 text-white text-sm rounded-full shadow-2xl opacity-0 transition-opacity pointer-events-none">
        추출이 완료되었습니다.
    </div>

    <script>
        const routeData = [
            // 동남아/서남아 (6)
            { region: "sea", port: "Port Kelang", country: "Malaysia", status: "Caution", lt: "10 ~ 14일", insight: "춘절 전 물량 집중으로 선복 확보 어려움. 포트 클랑은 싱가포르 대안으로 물량이 몰려 도착 후 반출 지연 가능성." },
            { region: "sea", port: "MANILA", country: "Philippines", status: "Normal", lt: "5 ~ 9일", insight: "북항/남항 운영 원활. 연초 수입 통관 강화 이슈가 간헐적으로 발생하므로 서류 준비 만전 필요." },
            { region: "sea", port: "BANGKOK", country: "Thailand", status: "Caution", lt: "12 ~ 16일", insight: "람차방의 환적 물류 증가로 바지선 연결 지연 가능성 상존. 직항보다는 환적 리스크 확인 필수." },
            { region: "sea", port: "SIHANOUKVILLE", country: "Cambodia", status: "Caution", lt: "14 ~ 18일", insight: "태국-캄보디아 국경 변수로 해상 의존도 심화. 환적항에서의 연결 지연 리스크 고려 필요." },
            { region: "sea", port: "JAKARTA", country: "Indonesia", status: "Caution", lt: "10 ~ 15일", insight: "탄중 프리옥 항만 혼잡도 상승. 세관 'Red Line' 검사 비율이 높아지는 시기이므로 통관 대비 요망." },
            { region: "sea", port: "SINGAPORE", country: "Singapore", status: "Normal", lt: "7 ~ 10일", insight: "환적 허브 효율 유지 중이나 춘절 전 화물 폭증으로 야적장 적체율 높음. 선복 확보는 용이." },

            // 오세아니아 (2)
            { region: "oceania", port: "MELBOURNE", country: "Australia", status: "Critical", lt: "18 ~ 28일 (+7일)", insight: "DP World/Patrick 파업으로 선박 체선 심각. 시드니 양하 후 내륙 운송 대안이나 파업 영향 적은 선사 검토." },
            { region: "oceania", port: "AUCKLAND", country: "New Zealand", region: "oceania", status: "Caution", lt: "20 ~ 30일", insight: "호주 항만 파업 여파가 오클랜드 향 서비스 지연으로 직결. 호주 미경유 직항 서비스 우선 확보 권장." },

            // 북미/남미 (8)
            { region: "na", port: "VANCOUVER", country: "Canada", status: "Caution", lt: "14 ~ 20일", insight: "터미널 내 철도 조차장 혼잡. 로컬 화물이라도 터미널 반출 속도가 느려질 수 있음에 유의." },
            { region: "na", port: "MISSISSAUGA (Rail)", country: "Canada (Toronto)", status: "Critical", lt: "35 ~ 50일", insight: "밴쿠버 철송 지연(평균 7.7일)과 혹한으로 인한 철도 운행 속도 저하 겹침. 납기 급한 화물 회피 권고." },
            { region: "na", port: "MISSISSAUGA (Truck)", country: "Canada (Vancouver)", status: "Critical", lt: "25 ~ 35일", insight: "로키 산맥 기상 악화로 도로 폐쇄 위험 높음. 비용이 높고 기상 변수가 크므로 긴급 물량만 고려." },
            { region: "na", port: "SEATTLE", country: "USA", status: "Normal", lt: "12 ~ 16일", insight: "캘리포니아 대비 혼잡도 낮고 철송 연결성 양호. 미 중서부 내륙 화물 진입 관문으로 추천." },
            { region: "na", port: "LONG BEACH", country: "USA", status: "Caution", lt: "12 ~ 18일", insight: "연말 물량 및 레일카 부족으로 터미널 체류 5~7일 증가. 트럭 게이트 예약 사전 배차 필요." },
            { region: "na", port: "NEW YORK", country: "USA", status: "Caution", lt: "28 ~ 40일", insight: "파나마 운하 제한 및 희망봉 우회 가능성 상존. 선박별 경유지에 따라 리드타임 편차 극심." },
            { region: "na", port: "SAVANNAH", country: "USA", status: "Caution", lt: "30 ~ 38일", insight: "운영 효율 높으나 우회 선박 일시 유입(Vessel Bunching) 발생 시 하역 지연 가능성." },
            { region: "na", port: "VITORIA", country: "Brazil", status: "Normal", lt: "35 ~ 45일", insight: "산토스 대비 혼잡도 낮음. 주로 산토스 등을 경유하므로 환적항 스케줄 밀착 관리 필요." },

            // 동아시아 (5)
            { region: "ea", port: "KAOHSIUNG", country: "Taiwan", status: "Normal", lt: "3 ~ 5일", insight: "환적항 운영 매우 안정적. 부산발 서비스 빈도 높아 선복 확보 용이." },
            { region: "ea", port: "KEELUNG", country: "Taiwan", status: "Normal", lt: "3 ~ 5일", insight: "타이베이 인근 항만으로 원활한 흐름 유지 중." },
            { region: "ea", port: "HONG KONG", country: "Hong Kong", status: "Normal", lt: "3 ~ 5일", insight: "춘절 전 중국 주강삼각주 피더 네트워크 지연 발생 가능성 상존." },
            { region: "ea", port: "YOKOHAMA", country: "Japan", status: "Normal", lt: "2 ~ 4일", insight: "매우 안정적인 루트. 특이사항 없음." },
            { region: "ea", port: "HAKATA", country: "Japan", status: "Normal", lt: "1 ~ 2일", insight: "페리 서비스 이용 시 당일/익일 통관 가능. 긴급 화물 처리에 최적화." },

            // 유럽/지중해 (3)
            { region: "eu", port: "SOUTHAMPTON", country: "UK", status: "Caution", lt: "40 ~ 50일", insight: "겨울철 기상 악화(강풍)로 인한 간헐적 운영 중단 리스크. 희망봉 우회로 LT 장기화." },
            { region: "eu", port: "ROTTERDAM", country: "Netherlands", status: "Caution", lt: "38 ~ 48일", insight: "겨울 폭풍 영향으로 터미널 효율 저하. 바지선 및 피더 연결 대기 시간이 길어져 환적 화물 추가 지연 불가피." },
            { region: "eu", port: "ISTANBUL", country: "Turkey", status: "Normal", lt: "35 ~ 45일", insight: "암바리 항만 큰 혼잡 없음. Middle Corridor 허브로서 전략적 가치 상승 중." },

            // 러시아/CIS (9)
            { region: "cis", port: "TOSHKENT", country: "Uzbekistan", status: "Caution", lt: "30 ~ 45일", insight: "중국 경유 TCR 루트. 중국-카자흐 국경 화차 교환 병목으로 국경 통과 7~10일 소요 가능성." },
            { region: "cis", port: "BISHKEK (TCR)", country: "Kyrgyzstan", status: "Caution", lt: "35 ~ 50일", insight: "동절기 폭설 시 국경 폐쇄 빈번. 추가적인 리드타임 확보 필수." },
            { region: "cis", port: "VLADIVOSTOK", country: "Russia", status: "Caution", lt: "2 ~ 5일", insight: "선복 제한적 및 고운임. 제재 강화로 선적 전 전략물자 서류 심사 매우 까다로움." },
            { region: "cis", port: "MOSCOW (TSR)", country: "Russia", status: "Critical", lt: "25 ~ 35일", insight: "RZD 화차 부족 및 군수 물자 우선 배정으로 민간 화물 철송 스케줄 불안정." },
            { region: "cis", port: "NOVOSIBIRSK (TSR)", country: "Russia", status: "Critical", lt: "20 ~ 30일", insight: "혹한기(-40도 이하) 장비 고장으로 인한 철송 지연 리스크 상시 존재." },
            { region: "cis", port: "MOSCOW (Truck)", country: "Russia", status: "Critical", lt: "18 ~ 25일", insight: "철송 대안이나 비용 높고 겨울철 도로 결빙/운전자 부족 리스크 큼. 긴급 화물만 고려." },
            { region: "cis", port: "NOVOSIBIRSK (Truck)", country: "Russia", status: "Critical", lt: "12 ~ 18일", insight: "장거리 운송 리스크. 화물 동결 파손 대비 위해 보온/냉장 트럭 사용 권장." },
            { region: "cis", port: "ALMATY (TCR)", country: "Kazakhstan", status: "Caution", lt: "25 ~ 35일", insight: "중앙아시아 물류 허브. 호르고스 국경 혼잡 예상되나 정책적 수혜로 타 CIS 대비 양호." },
            { region: "cis", port: "ULAANBAATAR", country: "Mongolia", status: "Caution", lt: "15 ~ 25일", insight: "중국 톈진항 적체 및 얼리안 국경 환적 지연이 상시적 리스크." }
        ];

        function renderRoutes(filter = "all", search = "") {
            const tbody = document.getElementById('routeTableBody');
            tbody.innerHTML = '';

            const filtered = routeData.filter(item => {
                const matchesFilter = filter === "all" || item.region === filter;
                const matchesSearch = item.port.toLowerCase().includes(search.toLowerCase()) || 
                                    item.country.toLowerCase().includes(search.toLowerCase());
                return matchesFilter && matchesSearch;
            });

            filtered.forEach((item, index) => {
                const row = document.createElement('tr');
                row.className = "hover:bg-slate-50 transition-colors cursor-pointer group";
                row.onclick = () => toggleRow(`detail-${index}`);

                let statusBadge = "";
                if(item.status === "Normal") statusBadge = `<span class="status-pill bg-green-100 text-green-700">Normal</span>`;
                else if(item.status === "Caution") statusBadge = `<span class="status-pill bg-amber-100 text-amber-700">Caution</span>`;
                else statusBadge = `<span class="status-pill bg-red-100 text-red-700">Critical</span>`;

                row.innerHTML = `
                    <td class="px-6 py-4 col-route">
                        <div class="text-slate-900 font-bold truncate">${item.port}</div>
                        <div class="text-[10px] text-slate-400 uppercase tracking-wider">${item.country}</div>
                    </td>
                    <td class="px-6 py-4 col-status">${statusBadge}</td>
                    <td class="px-6 py-4 col-lt">
                        <span class="text-sm text-slate-600 font-semibold nowrap">${item.lt}</span>
                    </td>
                    <td class="px-6 py-4 col-insight text-slate-400 text-sm italic">
                        <div class="flex items-center justify-between">
                            <span class="truncate pr-4">Click to view deep analysis...</span>
                            <i class="fas fa-chevron-down text-xs group-hover:text-indigo-500"></i>
                        </div>
                    </td>
                `;

                const detailRow = document.createElement('tr');
                detailRow.id = `detail-${index}`;
                detailRow.className = "detail-row";
                detailRow.innerHTML = `
                    <td colspan="4" class="px-10 py-6 border-b border-amber-100">
                        <div class="flex items-start gap-4">
                            <div class="w-10 h-10 bg-amber-200 rounded-xl flex items-center justify-center shrink-0">
                                <i class="fas fa-lightbulb text-amber-700"></i>
                            </div>
                            <div>
                                <p class="text-xs font-bold text-amber-800 uppercase tracking-widest mb-1">Expert Deep Insight</p>
                                <p class="text-sm text-slate-700 leading-relaxed font-medium">${item.insight}</p>
                            </div>
                        </div>
                    </td>
                `;

                tbody.appendChild(row);
                tbody.appendChild(detailRow);
            });
        }

        function toggleRow(id) {
            const row = document.getElementById(id);
            const isActive = row.classList.contains('active');
            
            // Close all others
            document.querySelectorAll('.detail-row').forEach(r => r.classList.remove('active'));
            
            if(!isActive) row.classList.add('active');
        }

        // HTML 추출 기능
        function exportToHTML() {
            const blob = new Blob([document.documentElement.outerHTML], { type: 'text/html' });
            const url = URL.createObjectURL(blob);
            const a = document.createElement('a');
            a.href = url;
            a.download = '2026_Jan_Logistics_Dashboard.html';
            a.click();
            URL.revokeObjectURL(url);
            showToast();
        }

        function exportToPDF() {
            const element = document.getElementById('captureArea');
            const opt = {
                margin: 10,
                filename: '2026_Jan_Logistics_Dashboard.pdf',
                image: { type: 'jpeg', quality: 0.98 },
                html2canvas: { scale: 2 },
                jsPDF: { unit: 'mm', format: 'a4', orientation: 'portrait' }
            };
            html2pdf().set(opt).from(element).save();
        }

        function showToast() {
            const t = document.getElementById("toast");
            t.style.opacity = "1";
            setTimeout(() => { t.style.opacity = "0"; }, 3000);
        }

        // Event Listeners
        document.getElementById('routeSearch').addEventListener('input', (e) => {
            const filter = document.getElementById('regionFilter').value;
            renderRoutes(filter, e.target.value);
        });

        document.getElementById('regionFilter').addEventListener('change', (e) => {
            const search = document.getElementById('routeSearch').value;
            renderRoutes(e.target.value, search);
        });

        // Initial Load
        window.onload = () => renderRoutes();

    </script>
</body>
</html>
