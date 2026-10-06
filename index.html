<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>카드 형식 메모장 - 마인드맵</title>
    
    <!-- Google Fonts: Pretendard (대체) + Inter -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&family=Noto+Sans+KR:wght@400;500;600;700&display=swap" rel="stylesheet">
    
    <style>
        /* =========================================
           1. 기본 스타일 및 변수 정의
           ========================================= */
        :root {
            --font-kr: 'Noto Sans KR', -apple-system, BlinkMacSystemFont, sans-serif;
            --font-en: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
            --bg-color: #f8f9fa;
            --card-bg: #ffffff;
            --text-main: #1a1a1a;
            --text-sub: #666666;
            --border-color: #e0e0e0;
            --primary-color: #4a90e2;
            --danger-color: #e74c3c;
            --radius: 12px;
            --shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
            --transition: all 0.2s ease;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: var(--font-en);
            background-color: var(--bg-color);
            color: var(--text-main);
            line-height: 1.6;
            padding: 20px;
            min-height: 100vh;
        }

        h1, h2, h3, .kr-text {
            font-family: var(--font-kr);
        }

        /* =========================================
           2. 레이아웃 및 헤더
           ========================================= */
        .container {
            max-width: 1400px;
            margin: 0 auto;
            position: relative;
        }

        header {
            text-align: center;
            margin-bottom: 40px;
            padding: 20px 0;
        }

        header h1 {
            font-size: 2rem;
            font-weight: 700;
            margin-bottom: 10px;
            color: var(--text-main);
        }

        .controls {
            display: flex;
            justify-content: center;
            gap: 12px;
            flex-wrap: wrap;
            margin-top: 20px;
        }

        /* =========================================
           3. 버튼 스타일
           ========================================= */
        button {
            font-family: var(--font-kr);
            padding: 10px 20px;
            border: none;
            border-radius: var(--radius);
            cursor: pointer;
            font-size: 0.95rem;
            font-weight: 500;
            transition: var(--transition);
            background-color: var(--card-bg);
            border: 1px solid var(--border-color);
            color: var(--text-main);
        }

        button:hover {
            background-color: var(--primary-color);
            color: white;
            border-color: var(--primary-color);
            transform: translateY(-2px);
            box-shadow: 0 4px 8px rgba(74, 144, 226, 0.2);
        }

        button.primary {
            background-color: var(--primary-color);
            color: white;
            border-color: var(--primary-color);
        }

        button.danger {
            color: var(--danger-color);
            border-color: var(--danger-color);
        }

        button.danger:hover {
            background-color: var(--danger-color);
            color: white;
        }

        /* =========================================
           4. 카드 그리드 및 드롭존
           ========================================= */
        .card-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 24px;
            padding: 20px 0 100px 0;
            position: relative;
            min-height: 600px;
        }

        /* 카드 스타일 */
        .card {
            background: var(--card-bg);
            border-radius: var(--radius);
            padding: 24px;
            box-shadow: var(--shadow);
            border: 1px solid var(--border-color);
            transition: var(--transition);
            position: relative;
            cursor: grab;
            display: flex;
            flex-direction: column;
            gap: 12px;
        }

        .card:hover {
            transform: translateY(-4px);
            box-shadow: 0 8px 24px rgba(0, 0, 0, 0.12);
        }

        .card.dragging {
            opacity: 0.5;
            cursor: grabbing;
        }

        /* 카드 헤더 (분류 + 액션) */
        .card-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 8px;
        }

        .card-category {
            font-size: 0.85rem;
            font-weight: 600;
            color: var(--text-sub);
            background: #f0f0f0;
            padding: 4px 10px;
            border-radius: 6px;
        }

        .card-actions {
            display: flex;
            gap: 6px;
        }

        .card-actions button {
            padding: 4px 8px;
            font-size: 0.75rem;
            min-height: 28px;
        }

        /* 카드 내용 */
        .card-content {
            font-size: 1rem;
            line-height: 1.6;
            color: var(--text-main);
            flex-grow: 1;
            white-space: pre-wrap;
            word-break: break-word;
        }

        /* 카드 푸터 (출처) */
        .card-footer {
            margin-top: auto;
            display: flex;
            align-items: center;
            gap: 8px;
            font-size: 0.8rem;
            color: #999;
        }

        .source-link {
            color: #999;
            text-decoration: none;
            display: inline-flex;
            align-items: center;
            gap: 4px;
            transition: var(--transition);
        }

        .source-link:hover {
            color: var(--primary-color);
        }

        .source-link svg {
            width: 14px;
            height: 14px;
        }

        /* =========================================
           5. 연결선 (SVG)
           ========================================= */
        #connections-layer {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 0;
        }

        .connection-line {
            stroke: var(--text-sub);
            stroke-width: 2;
            fill: none;
            opacity: 0.4;
        }

        /* =========================================
           6. 요약 피드백 섹션
           ========================================= */
        .summary-section {
            background: white;
            border-radius: var(--radius);
            padding: 30px;
            margin-top: 40px;
            box-shadow: var(--shadow);
            border: 1px solid var(--border-color);
        }

        .summary-section h2 {
            font-size: 1.5rem;
            margin-bottom: 16px;
            color: var(--text-main);
        }

        .summary-content {
            font-size: 1rem;
            color: var(--text-sub);
            line-height: 1.8;
        }

        /* =========================================
           7. 반응형 디자인 (미디어 쿼리)
           ========================================= */
        
        /* 태블릿: 641px ~ 1024px (한 줄 2 개) */
        @media (max-width: 1024px) {
            .card-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        /* 모바일: 최대 640px (한 줄 1 개) */
        @media (max-width: 640px) {
            body {
                padding: 16px;
            }

            .card-grid {
                grid-template-columns: 1fr;
                gap: 16px;
            }

            header h1 {
                font-size: 1.5rem;
            }

            /* 모바일 버튼 터치 최적화 */
            button {
                min-height: 48px;
                padding: 12px 20px;
            }

            .card {
                padding: 20px;
            }

            .card-content {
                font-size: 16px; /* 가독성 유지 */
            }

            .summary-section {
                padding: 20px;
            }
        }

        /* 이미지 자동 축소 */
        img {
            max-width: 100%;
            height: auto;
            border-radius: 8px;
        }

        /* =========================================
           8. 모달 (카드 추가/수정)
           ========================================= */
        .modal-overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.5);
            display: none;
            justify-content: center;
            align-items: center;
            z-index: 1000;
            backdrop-filter: blur(4px);
        }

        .modal-overlay.active {
            display: flex;
        }

        .modal {
            background: white;
            border-radius: var(--radius);
            padding: 30px;
            width: 90%;
            max-width: 500px;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.2);
            animation: modalSlideIn 0.3s ease;
        }

        @keyframes modalSlideIn {
            from {
                opacity: 0;
                transform: translateY(-20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .modal h3 {
            font-size: 1.25rem;
            margin-bottom: 20px;
        }

        .form-group {
            margin-bottom: 16px;
        }

        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
            color: var(--text-main);
        }

        .form-group input,
        .form-group textarea,
        .form-group select {
            width: 100%;
            padding: 12px;
            border: 1px solid var(--border-color);
            border-radius: 8px;
            font-family: var(--font-kr);
            font-size: 1rem;
            transition: var(--transition);
        }

        .form-group input:focus,
        .form-group textarea:focus,
        .form-group select:focus {
            outline: none;
            border-color: var(--primary-color);
            box-shadow: 0 0 0 3px rgba(74, 144, 226, 0.1);
        }

        .form-group textarea {
            min-height: 120px;
            resize: vertical;
        }

        .modal-actions {
            display: flex;
            justify-content: flex-end;
            gap: 12px;
            margin-top: 24px;
        }

        /* 색상 선택기 */
        .color-picker {
            display: flex;
            gap: 8px;
            flex-wrap: wrap;
        }

        .color-option {
            width: 32px;
            height: 32px;
            border-radius: 50%;
            cursor: pointer;
            border: 2px solid transparent;
            transition: var(--transition);
        }

        .color-option:hover,
        .color-option.selected {
            transform: scale(1.1);
            border-color: var(--text-main);
        }

        /* 연결 모드 활성화 시 */
        body.connect-mode .card {
            cursor: crosshair;
        }

        body.connect-mode .card.connecting {
            border: 2px dashed var(--primary-color);
            background-color: rgba(74, 144, 226, 0.05);
        }

        body.connect-mode .card.connected {
            border: 2px solid var(--primary-color);
        }
    </style>
</head>
<body>

    <div class="container">
        <!-- 헤더 섹션 -->
        <header>
            <h1>📝 카드 형식 메모장</h1>
            <p class="kr-text" style="color: var(--text-sub);">아이디어를 카드에 적고, 연결하며 흐름을 만들어보세요.</p>
            
            <div class="controls">
                <button class="primary" id="addCardBtn">+ 새 카드 추가</button>
                <button id="connectModeBtn">🔗 연결 모드</button>
                <button id="clearConnectionsBtn">연결선 초기화</button>
                <button id="generateSummaryBtn">📊 흐름 요약하기</button>
            </div>
        </header>

        <!-- 카드 그리드 영역 -->
        <div class="card-grid" id="cardGrid">
            <!-- SVG 연결선 레이어 -->
            <svg id="connections-layer"></svg>
            <!-- 카드들은 JavaScript 로 동적 추가됨 -->
        </div>

        <!-- 요약 피드백 섹션 -->
        <section class="summary-section">
            <h2>💡 흐름 요약</h2>
            <div class="summary-content kr-text" id="summaryContent">
                카드를 연결하고 '흐름 요약하기' 버튼을 누르면 여기에 분석 결과가 표시됩니다.
            </div>
        </section>
    </div>

    <!-- 카드 추가/수정 모달 -->
    <div class="modal-overlay" id="cardModal">
        <div class="modal">
            <h3 class="kr-text" id="modalTitle">새 카드 추가</h3>
            <form id="cardForm">
                <input type="hidden" id="cardId">
                
                <div class="form-group">
                    <label for="cardCategory" class="kr-text">분류</label>
                    <input type="text" id="cardCategory" placeholder="예: 아이디어, 참고자료, 질문" required>
                </div>

                <div class="form-group">
                    <label for="cardContent" class="kr-text">내용</label>
                    <textarea id="cardContent" placeholder="여기에 내용을 입력하세요..." required></textarea>
                </div>

                <div class="form-group">
                    <label for="cardSource" class="kr-text">출처</label>
                    <input type="text" id="cardSource" placeholder="예: 위키백과, 논문 제목">
                </div>

                <div class="form-group">
                    <label for="cardUrl" class="kr-text">URL (선택)</label>
                    <input type="url" id="cardUrl" placeholder="https://example.com">
                </div>

                <div class="form-group">
                    <label class="kr-text">배경색</label>
                    <div class="color-picker" id="colorPicker">
                        <div class="color-option selected" data-color="#ffffff" style="background: #ffffff; border: 1px solid #ddd;"></div>
                        <div class="color-option" data-color="#fff3cd" style="background: #fff3cd;"></div>
                        <div class="color-option" data-color="#d4edda" style="background: #d4edda;"></div>
                        <div class="color-option" data-color="#d1ecf1" style="background: #d1ecf1;"></div>
                        <div class="color-option" data-color="#f8d7da" style="background: #f8d7da;"></div>
                        <div class="color-option" data-color="#e2e3e5" style="background: #e2e3e5;"></div>
                    </div>
                </div>

                <div class="modal-actions">
                    <button type="button" id="cancelBtn">취소</button>
                    <button type="submit" class="primary">저장</button>
                </div>
            </form>
        </div>
    </div>

    <script>
        /* =========================================
           JavaScript 동작 로직
           ========================================= */

        // 1. 상태 관리 (State Management)
        const state = {
            cards: [],
            connections: [], // {from: cardId, to: cardId}
            isConnectMode: false,
            selectedCardForConnection: null,
            nextId: 1,
            selectedColor: '#ffffff'
        };

        // 2. DOM 요소 참조
        const cardGrid = document.getElementById('cardGrid');
        const cardModal = document.getElementById('cardModal');
        const cardForm = document.getElementById('cardForm');
        const modalTitle = document.getElementById('modalTitle');
        const colorPicker = document.getElementById('colorPicker');
        const summaryContent = document.getElementById('summaryContent');
        const svgLayer = document.getElementById('connections-layer');

        // 3. 유틸리티 함수
        const generateId = () => `card_${Date.now()}_${state.nextId++}`;
        
        const escapeHtml = (text) => {
            if (!text) return '';
            return text.replace(/&/g, '&amp;').replace(/</g, '&lt;').replace(/>/g, '&gt;');
        };

        // 4. 카드 렌더링 함수
        const renderCard = (card) => {
            const cardEl = document.createElement('div');
            cardEl.className = 'card';
            cardEl.id = card.id;
            cardEl.draggable = true;
            cardEl.style.backgroundColor = card.color;
            cardEl.dataset.id = card.id;

            // 출처 링크 처리
            let sourceHtml = '';
            if (card.url) {
                sourceHtml = `
                    <a href="${escapeHtml(card.url)}" target="_blank" class="source-link" title="출처 바로가기">
                        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                            <path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path>
                            <path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path>
                        </svg>
                    </a>
                `;
            }

            cardEl.innerHTML = `
                <div class="card-header">
                    <span class="card-category">${escapeHtml(card.category)}</span>
                    <div class="card-actions">
                        <button class="edit-btn" data-id="${card.id}">수정</button>
                        <button class="danger delete-btn" data-id="${card.id}">삭제</button>
                    </div>
                </div>
                <div class="card-content kr-text">${escapeHtml(card.content)}</div>
                <div class="card-footer">
                    <span>${escapeHtml(card.source)}</span>
                    ${sourceHtml}
                </div>
            `;

            // 드래그 앤 드롭 이벤트 리스너
            addDragEvents(cardEl);

            // 클릭 이벤트 (연결 모드)
            cardEl.addEventListener('click', (e) => {
                if (state.isConnectMode && !e.target.closest('button')) {
                    handleCardClickForConnection(card.id);
                }
            });

            // 수정/삭제 버튼 이벤트
            cardEl.querySelector('.edit-btn').addEventListener('click', () => openEditModal(card.id));
            cardEl.querySelector('.delete-btn').addEventListener('click', () => deleteCard(card.id));

            return cardEl;
        };

        const renderAllCards = () => {
            // 기존 카드 제거 (SVG 는 유지)
            const existingCards = cardGrid.querySelectorAll('.card');
            existingCards.forEach(card => card.remove());

            // 새 카드 렌더링
            state.cards.forEach(card => {
                cardGrid.appendChild(renderCard(card));
            });

            // 연결선 다시 그리기
            requestAnimationFrame(drawConnections);
        };

        // 5. 모달 관련 함수
        const openAddModal = () => {
            modalTitle.textContent = '새 카드 추가';
            cardForm.reset();
            document.getElementById('cardId').value = '';
            state.selectedColor = '#ffffff';
            updateColorPickerSelection();
            cardModal.classList.add('active');
        };

        const openEditModal = (cardId) => {
            const card = state.cards.find(c => c.id === cardId);
            if (!card) return;

            modalTitle.textContent = '카드 수정';
            document.getElementById('cardId').value = card.id;
            document.getElementById('cardCategory').value = card.category;
            document.getElementById('cardContent').value = card.content;
            document.getElementById('cardSource').value = card.source;
            document.getElementById('cardUrl').value = card.url;
            state.selectedColor = card.color;
            updateColorPickerSelection();
            cardModal.classList.add('active');
        };

        const closeModal = () => {
            cardModal.classList.remove('active');
        };

        // 6. 색상 선택기 로직
        const updateColorPickerSelection = () => {
            const options = colorPicker.querySelectorAll('.color-option');
            options.forEach(opt => {
                if (opt.dataset.color === state.selectedColor) {
                    opt.classList.add('selected');
                } else {
                    opt.classList.remove('selected');
                }
            });
        };

        colorPicker.querySelectorAll('.color-option').forEach(opt => {
            opt.addEventListener('click', () => {
                state.selectedColor = opt.dataset.color;
                updateColorPickerSelection();
            });
        });

        // 7. 카드 CRUD 연산
        const saveCard = (e) => {
            e.preventDefault();
            
            const cardId = document.getElementById('cardId').value;
            const category = document.getElementById('cardCategory').value;
            const content = document.getElementById('cardContent').value;
            const source = document.getElementById('cardSource').value;
            const url = document.getElementById('cardUrl').value;
            const color = state.selectedColor;

            if (cardId) {
                // 수정
                const index = state.cards.findIndex(c => c.id === cardId);
                if (index !== -1) {
                    state.cards[index] = { ...state.cards[index], category, content, source, url, color };
                }
            } else {
                // 추가
                const newCard = {
                    id: generateId(),
                    category,
                    content,
                    source,
                    url,
                    color
                };
                state.cards.push(newCard);
            }

            renderAllCards();
            closeModal();
        };

        const deleteCard = (cardId) => {
            if (!confirm('정말 이 카드를 삭제하시겠습니까?')) return;
            
            state.cards = state.cards.filter(c => c.id !== cardId);
            // 관련 연결선도 제거
            state.connections = state.connections.filter(conn => 
                conn.from !== cardId && conn.to !== cardId
            );
            
            renderAllCards();
        };

        // 8. 드래그 앤 드롭 (순수 JS)
        let draggedCard = null;

        const addDragEvents = (card) => {
            card.addEventListener('dragstart', (e) => {
                draggedCard = card;
                card.classList.add('dragging');
                e.dataTransfer.effectAllowed = 'move';
                // 드래그 이미지 설정 (선택사항)
                e.dataTransfer.setData('text/plain', card.id);
            });

            card.addEventListener('dragend', () => {
                card.classList.remove('dragging');
                draggedCard = null;
            });

            card.addEventListener('dragover', (e) => {
                e.preventDefault(); // 드롭 허용
                e.dataTransfer.dropEffect = 'move';
            });

            card.addEventListener('drop', (e) => {
                e.preventDefault();
                if (draggedCard && draggedCard !== card) {
                    // 순서 변경 로직
                    const fromIndex = state.cards.findIndex(c => c.id === draggedCard.dataset.id);
                    const toIndex = state.cards.findIndex(c => c.id === card.dataset.id);
                    
                    if (fromIndex !== -1 && toIndex !== -1) {
                        const [movedCard] = state.cards.splice(fromIndex, 1);
                        state.cards.splice(toIndex, 0, movedCard);
                        renderAllCards();
                    }
                }
            });
        };

        // 그리드 자체에도 드롭 이벤트 추가 (맨 끝으로 이동)
        cardGrid.addEventListener('dragover', (e) => {
            e.preventDefault();
        });

        cardGrid.addEventListener('drop', (e) => {
            if (e.target === cardGrid && draggedCard) {
                const fromIndex = state.cards.findIndex(c => c.id === draggedCard.dataset.id);
                if (fromIndex !== -1) {
                    const [movedCard] = state.cards.splice(fromIndex, 1);
                    state.cards.push(movedCard);
                    renderAllCards();
                }
            }
        });

        // 9. 연결선 기능 (SVG)
        const handleCardClickForConnection = (cardId) => {
            if (!state.isConnectMode) return;

            if (!state.selectedCardForConnection) {
                // 첫 번째 카드 선택
                state.selectedCardForConnection = cardId;
                document.getElementById(cardId).classList.add('connecting');
            } else {
                // 두 번째 카드 선택 (연결 완료)
                if (state.selectedCardForConnection !== cardId) {
                    // 중복 연결 확인
                    const exists = state.connections.some(conn => 
                        (conn.from === state.selectedCardForConnection && conn.to === cardId) ||
                        (conn.from === cardId && conn.to === state.selectedCardForConnection)
                    );

                    if (!exists) {
                        state.connections.push({
                            from: state.selectedCardForConnection,
                            to: cardId
                        });
                        drawConnections();
                    }
                }
                // 초기화
                document.getElementById(state.selectedCardForConnection)?.classList.remove('connecting');
                state.selectedCardForConnection = null;
            }
        };

        const drawConnections = () => {
            // 기존 선 제거
            svgLayer.innerHTML = '';
            
            const gridRect = cardGrid.getBoundingClientRect();

            state.connections.forEach(conn => {
                const fromCard = document.getElementById(conn.from);
                const toCard = document.getElementById(conn.to);

                if (!fromCard || !toCard) return;

                const fromRect = fromCard.getBoundingClientRect();
                const toRect = toCard.getBoundingClientRect();

                // 카드 중심점 계산 (그리드 기준 상대 좌표)
                const x1 = fromRect.left + fromRect.width / 2 - gridRect.left;
                const y1 = fromRect.top + fromRect.height / 2 - gridRect.top;
                const x2 = toRect.left + toRect.width / 2 - gridRect.left;
                const y2 = toRect.top + toRect.height / 2 - gridRect.top;

                // SVG 선 생성
                const line = document.createElementNS('http://www.w3.org/2000/svg', 'line');
                line.setAttribute('x1', x1);
                line.setAttribute('y1', y1);
                line.setAttribute('x2', x2);
                line.setAttribute('y2', y2);
                line.classList.add('connection-line');

                svgLayer.appendChild(line);
            });
        };

        // 10. 요약 생성 기능 (단순 로직)
        const generateSummary = () => {
            if (state.cards.length === 0) {
                summaryContent.textContent = '카드가 없습니다. 먼저 카드를 추가해주세요.';
                return;
            }

            const connectedCardIds = new Set();
            state.connections.forEach(conn => {
                connectedCardIds.add(conn.from);
                connectedCardIds.add(conn.to);
            });

            const connectedCards = state.cards.filter(c => connectedCardIds.has(c.id));
            const isolatedCards = state.cards.filter(c => !connectedCardIds.has(c.id));

            let summaryText = `<strong>총 ${state.cards.length}개의 카드</strong> 중 <strong>${connectedCards.length}개</strong>가 연결되었습니다.<br><br>`;

            if (connectedCards.length > 0) {
                summaryText += `<strong>🔗 연결된 흐름:</strong><br>`;
                connectedCards.forEach((card, idx) => {
                    summaryText += `${idx + 1}. [${card.category}] ${card.content.substring(0, 30)}...<br>`;
                });
                summaryText += `<br>`;
            }

            if (isolatedCards.length > 0) {
                summaryText += `<strong>📌 고립된 카드 (연결 필요):</strong><br>`;
                isolatedCards.forEach(card => {
                    summaryText += `- [${card.category}] ${card.content.substring(0, 20)}...<br>`;
                });
            }

            if (state.connections.length === 0 && state.cards.length > 0) {
                summaryText = '카드가 있지만 연결된 것이 없습니다. "연결 모드"를 사용하여 카드를 연결해보세요!';
            }

            summaryContent.innerHTML = summaryText;
        };

        // 11. 이벤트 리스너 등록
        document.getElementById('addCardBtn').addEventListener('click', openAddModal);
        document.getElementById('cancelBtn').addEventListener('click', closeModal);
        cardForm.addEventListener('submit', saveCard);

        document.getElementById('connectModeBtn').addEventListener('click', () => {
            state.isConnectMode = !state.isConnectMode;
            document.body.classList.toggle('connect-mode', state.isConnectMode);
            document.getElementById('connectModeBtn').textContent = 
                state.isConnectMode ? '✅ 연결 모드 종료' : '🔗 연결 모드';
            
            // 모드 종료 시 선택 초기화
            if (!state.isConnectMode && state.selectedCardForConnection) {
                document.getElementById(state.selectedCardForConnection)?.classList.remove('connecting');
                state.selectedCardForConnection = null;
            }
        });

        document.getElementById('clearConnectionsBtn').addEventListener('click', () => {
            if (confirm('모든 연결선을 삭제하시겠습니까?')) {
                state.connections = [];
                drawConnections();
            }
        });

        document.getElementById('generateSummaryBtn').addEventListener('click', generateSummary);

        // 모달 바깥 클릭 시 닫기
        cardModal.addEventListener('click', (e) => {
            if (e.target === cardModal) {
                closeModal();
            }
        });

        // 12. 초기 샘플 데이터 (테스트용)
        const initSampleData = () => {
            state.cards = [
                {
                    id: generateId(),
                    category: '아이디어',
                    content: '온라인 커뮤니티에서 학습자가 서로의 의견을 주고받는 과정이 중요함.',
                    source: 'CSCL 이론',
                    url: 'https://en.wikipedia.org/wiki/Computer-supported_collaborative_learning',
                    color: '#d1ecf1'
                },
                {
                    id: generateId(),
                    category: '참고자료',
                    content: '팬덤 커뮤니티의 협력적 활동이 비공식 학습 환경으로 작용할 수 있다는 연구.',
                    source: '학위논문',
                    url: '',
                    color: '#fff3cd'
                },
                {
                    id: generateId(),
                    category: '질문',
                    content: '어떻게 하면 감정 조절을 지원하는 도구를 설계할 수 있을까?',
                    source: '연구 노트',
                    url: '',
                    color: '#ffffff'
                }
            ];
            renderAllCards();
        };

        // 페이지 로드 시 초기화
        window.addEventListener('DOMContentLoaded', () => {
            initSampleData();
            
            // 윈도우 리사이즈 시 연결선 다시 그리기
            window.addEventListener('resize', () => {
                requestAnimationFrame(drawConnections);
            });
        });

    </script>
</body>
</html>
