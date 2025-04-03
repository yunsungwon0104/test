<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>스마트 신발: 자동 굽 조절 시스템 대시보드</title>
    <style>
        :root {
            --primary: #3498db;
            --secondary: #2ecc71;
            --dark: #2c3e50;
            --light: #ecf0f1;
            --warning: #e74c3c;
        }
        
        body {
            font-family: 'Noto Sans KR', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f5f5f5;
            color: var(--dark);
        }
        
        header {
            background-color: var(--primary);
            color: white;
            padding: 1rem;
            text-align: center;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        .dashboard {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
        }
        
        @media (max-width: 768px) {
            .dashboard {
                grid-template-columns: 1fr;
            }
        }
        
        .card {
            background: white;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            padding: 20px;
            margin-bottom: 20px;
        }
        
        .full-width {
            grid-column: 1 / -1;
        }
        
        h2 {
            color: var(--primary);
            border-bottom: 2px solid var(--light);
            padding-bottom: 10px;
            margin-top: 0;
        }
        
        .status-indicator {
            display: inline-block;
            width: 12px;
            height: 12px;
            border-radius: 50%;
            margin-right: 8px;
        }
        
        .status-active {
            background-color: var(--secondary);
        }
        
        .status-inactive {
            background-color: var(--warning);
        }
        
        .data-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 15px;
            margin-top: 15px;
        }
        
        .data-item {
            text-align: center;
            padding: 15px;
            background-color: #f9f9f9;
            border-radius: 6px;
        }
        
        .data-value {
            font-size: 1.8rem;
            font-weight: bold;
            color: var(--primary);
            margin: 5px 0;
        }
        
        .data-label {
            font-size: 0.9rem;
            color: #777;
        }
        
        #map {
            height: 300px;
            background-color: #e0e0e0;
            border-radius: 8px;
            margin-top: 15px;
        }
        
        .chart-container {
            height: 250px;
            position: relative;
            margin-top: 15px;
        }
        
        button {
            background-color: var(--primary);
            color: white;
            border: none;
            padding: 10px 15px;
            border-radius: 4px;
            cursor: pointer;
            margin-right: 10px;
            transition: background-color 0.3s;
        }
        
        button:hover {
            background-color: #2980b9;
        }
        
        .controls {
            margin-top: 20px;
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }
        
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 15px;
        }
        
        table th, table td {
            padding: 10px;
            text-align: left;
            border-bottom: 1px solid #ddd;
        }
        
        table th {
            background-color: #f2f2f2;
        }
        
        .shoe-diagram {
            display: flex;
            justify-content: center;
            margin: 20px 0;
        }
        
        .shoe {
            position: relative;
            width: 300px;
            height: 200px;
            background-color: #f0f0f0;
            border-radius: 10px;
            display: flex;
            justify-content: center;
            align-items: center;
        }
        
        .heel {
            position: absolute;
            bottom: 0;
            width: 80px;
            height: 40px;
            background-color: var(--primary);
            border-radius: 5px 5px 0 0;
            transform-origin: bottom;
            transform: translateY(20px);
            transition: transform 0.5s;
        }
        
        #notifications {
            max-height: 200px;
            overflow-y: auto;
        }
        
        .notification {
            padding: 10px;
            margin-bottom: 8px;
            border-radius: 4px;
            background-color: #f0f0f0;
        }
        
        .notification.warning {
            background-color: #ffeaa7;
        }
        
        .notification.success {
            background-color: #d5f5e3;
        }
    </style>
</head>
<body>
    <header>
        <h1>스마트 신발: 자동 굽 조절 시스템 대시보드</h1>
    </header>
    
    <div class="container">
        <div class="card full-width">
            <h2>시스템 상태</h2>
            <div class="data-grid">
                <div class="data-item">
                    <div class="data-label">라즈베리파이 상태</div>
                    <div class="data-value">
                        <span class="status-indicator status-active"></span>온라인
                    </div>
                </div>
                <div class="data-item">
                    <div class="data-label">배터리</div>
                    <div class="data-value">85%</div>
                </div>
                <div class="data-item">
                    <div class="data-label">자이로스코프</div>
                    <div class="data-value">
                        <span class="status-indicator status-active"></span>연결됨
                    </div>
                </div>
                <div class="data-item">
                    <div class="data-label">GPS</div>
                    <div class="data-value">
                        <span class="status-indicator status-active"></span>연결됨
                    </div>
                </div>
            </div>
        </div>
        
        <div class="dashboard">
            <div class="card">
                <h2>실시간 경사도 및 굽 조절</h2>
                <div class="data-grid">
                    <div class="data-item">
                        <div class="data-label">현재 경사각</div>
                        <div class="data-value">5.2°</div>
                    </div>
                    <div class="data-item">
                        <div class="data-label">굽 높이</div>
                        <div class="data-value">2.8cm</div>
                    </div>
                </div>
                
                <div class="shoe-diagram">
                    <div class="shoe">
                        <div class="heel" id="heel" style="transform: rotate(5.2deg) translateY(20px);"></div>
                    </div>
                </div>
                
                <div class="controls">
                    <button onclick="adjustHeel('up')">굽 높이 증가</button>
                    <button onclick="adjustHeel('down')">굽 높이 감소</button>
                    <button onclick="toggleAutoMode()">자동 모드 전환</button>
                </div>
            </div>
            
            <div class="card">
                <h2>보행 패턴 분석</h2>
                <div class="chart-container">
                    <!-- 보행 패턴 차트가 들어갈 위치 -->
                    <img src="/api/placeholder/500/250" alt="보행 패턴 차트">
                </div>
                <div class="data-grid">
                    <div class="data-item">
                        <div class="data-label">보폭 수</div>
                        <div class="data-value">1,248</div>
                    </div>
                    <div class="data-item">
                        <div class="data-label">평균 보폭</div>
                        <div class="data-value">73cm</div>
                    </div>
                    <div class="data-item">
                        <div class="data-label">칼로리</div>
                        <div class="data-value">287</div>
                    </div>
                </div>
            </div>
            
            <div class="card">
                <h2>지형 및 GPS 정보</h2>
                <div id="map">
                    <!-- 지도가 들어갈 위치 -->
                    <img src="/api/placeholder/500/300" alt="GPS 지도">
                </div>
                <div class="data-grid">
                    <div class="data-item">
                        <div class="data-label">평균 경사도</div>
                        <div class="data-value">3.8°</div>
                    </div>
                    <div class="data-item">
                        <div class="data-label">이동 거리</div>
                        <div class="data-value">2.4km</div>
                    </div>
                    <div class="data-item">
                        <div class="data-label">예상 도착</div>
                        <div class="data-value">14분</div>
                    </div>
                </div>
            </div>
            
            <div class="card">
                <h2>시스템 알림</h2>
                <div id="notifications">
                    <div class="notification success">
                        <strong>14:32</strong> - 경사 변화 감지: 굽 높이 자동 조정 (2.5cm → 2.8cm)
                    </div>
                    <div class="notification">
                        <strong>14:15</strong> - 평지 감지: 기본 굽 높이로 설정 (2.5cm)
                    </div>
                    <div class="notification warning">
                        <strong>13:58</strong> - 높은 경사 감지 (7.5°): 주의 필요
                    </div>
                    <div class="notification">
                        <strong>13:45</strong> - 시스템 시작: 자동 조절 모드 활성화
                    </div>
                </div>
            </div>
        </div>
        
        <div class="card full-width">
            <h2>모터 및 센서 상태</h2>
            <table>
                <thead>
                    <tr>
                        <th>구성 요소</th>
                        <th>상태</th>
                        <th>값</th>
                        <th>배터리 소모</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>MPU-6050 센서</td>
                        <td><span class="status-indicator status-active"></span> 정상</td>
                        <td>X: 0.2, Y: 5.2, Z: 0.1</td>
                        <td>낮음</td>
                    </tr>
                    <tr>
                        <td>서보모터 (MG996R)</td>
                        <td><span class="status-indicator status-active"></span> 정상</td>
                        <td>PWM: 1500μs</td>
                        <td>중간</td>
                    </tr>
                    <tr>
                        <td>압력 센서</td>
                        <td><span class="status-indicator status-active"></span> 정상</td>
                        <td>75kg</td>
                        <td>낮음</td>
                    </tr>
                    <tr>
                        <td>Raspberry Pi Zero 2 W</td>
                        <td><span class="status-indicator status-active"></span> 정상</td>
                        <td>CPU: 15%, Temp: 42°C</td>
                        <td>중간</td>
                    </tr>
                </tbody>
            </table>
        </div>
    </div>

    <script>
        // 데모용 스크립트 - 실제 구현에서는 라즈베리파이와 통신 필요
        let autoMode = true;
        let currentAngle = 5.2;
        
        function adjustHeel(direction) {
            const heel = document.getElementById('heel');
            if (direction === 'up') {
                currentAngle += 1;
                if (currentAngle > 15) currentAngle = 15;
            } else {
                currentAngle -= 1;
                if (currentAngle < 0) currentAngle = 0;
            }
            
            heel.style.transform = `rotate(${currentAngle}deg) translateY(20px)`;
            
            // 알림 추가
            addNotification(`굽 높이 수동 조절: ${currentAngle.toFixed(1)}°`, 'normal');
        }
        
        function toggleAutoMode() {
            autoMode = !autoMode;
            const status = autoMode ? '활성화' : '비활성화';
            addNotification(`자동 모드 ${status}`, autoMode ? 'success' : 'warning');
        }
        
        function addNotification(message, type = 'normal') {
            const notifications = document.getElementById('notifications');
            const now = new Date();
            const time = `${now.getHours()}:${now.getMinutes().toString().padStart(2, '0')}`;
            
            const notification = document.createElement('div');
            notification.className = `notification ${type}`;
            notification.innerHTML = `<strong>${time}</strong> - ${message}`;
            
            notifications.insertBefore(notification, notifications.firstChild);
        }
        
        // 시뮬레이션: 임의의 경사 변화에 따른 굽 높이 조절
        setInterval(() => {
            if (autoMode) {
                const randomChange = (Math.random() - 0.5) * 2;
                currentAngle += randomChange;
                if (currentAngle < 0) currentAngle = 0;
                if (currentAngle > 15) currentAngle = 15;
                
                document.getElementById('heel').style.transform = `rotate(${currentAngle}deg) translateY(20px)`;
                
                // 경사 값 업데이트
                document.querySelectorAll('.data-value')[2].textContent = `${currentAngle.toFixed(1)}°`;
                
                // 굽 높이 업데이트 (경사에 비례)
                const heelHeight = 2 + (currentAngle / 10);
                document.querySelectorAll('.data-value')[3].textContent = `${heelHeight.toFixed(1)}cm`;
                
                // 큰 변화가 있을 때만 알림 추가
                if (Math.abs(randomChange) > 1) {
                    addNotification(`경사 변화 감지: 굽 높이 자동 조정 (${heelHeight.toFixed(1)}cm)`, 'success');
                }
            }
        }, 5000);
    </script>
</body>
</html>
