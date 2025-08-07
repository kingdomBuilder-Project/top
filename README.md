<!DOCTYPE html>
<html lang="ko" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>킹덤 빌더 | 당신의 삶을 재건축하는 12가지 설계도</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@400;700&family=Gowun+Batang:wght@700&display=swap" rel="stylesheet">
    
    <!-- Chosen Palette: Scribe's Parchment (#FBF8F1, #3D3A37, #A9A299, #DAA520) -->
    <!-- Application Structure Plan: A single-page, vertical-scrolling application structured into the book's 4 parts. Interactive chapter cards open modals with detailed summaries, allowing for focused exploration. This structure was chosen to guide the user through the book's linear progression in an engaging, non-overwhelming way, mirroring the experience of building something step-by-step. -->
    <!-- Visualization & Content Choices: Report Info: 12 Chapters in 4 Parts. Goal: Organize, explain, and engage. Viz/Method: Interactive cards (HTML/CSS/JS) for chapters. Interaction: Clicking cards opens modals. Justification: This card/modal system presents a large amount of text content in a digestible, user-controlled manner, preventing information overload on the main page and allowing for deeper dives into specific topics. Library/Method: Vanilla JS for all interactions, Tailwind CSS for styling. -->
    <!-- CONFIRMATION: NO SVG graphics used. NO Mermaid JS used. -->

    <style>
        body {
            font-family: 'Noto Sans KR', sans-serif;
            background-color: #FBF8F1;
            color: #3D3A37;
        }
        .font-display {
            font-family: 'Gowun Batang', serif;
            font-weight: 700;
        }
        .card-hover {
            transition: all 0.3s ease-in-out;
        }
        .card-hover:hover {
            transform: translateY(-8px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
        }
        .modal-backdrop {
            transition: opacity 0.3s ease-in-out;
        }
        .modal-content {
            transition: all 0.3s ease-in-out;
        }
    </style>
</head>
<body class="antialiased">

    <header class="bg-white/80 backdrop-blur-lg sticky top-0 z-40 w-full border-b border-stone-200">
        <div class="container mx-auto px-4 sm:px-6 lg:px-8 flex items-center justify-between h-16">
            <a href="#" class="text-2xl font-display text-stone-800">킹덤 빌더</a>
            <nav class="hidden md:flex space-x-8">
                <a href="#part1" class="font-bold text-stone-600 hover:text-amber-600 transition-colors">기초</a>
                <a href="#part2" class="font-bold text-stone-600 hover:text-amber-600 transition-colors">설계</a>
                <a href="#part3" class="font-bold text-stone-600 hover:text-amber-600 transition-colors">엔진</a>
                <a href="#part4" class="font-bold text-stone-600 hover:text-amber-600 transition-colors">완성</a>
            </nav>
        </div>
    </header>

    <main>
        <section class="py-20 sm:py-32 bg-white">
            <div class="container mx-auto px-4 sm:px-6 lg:px-8 text-center">
                <h1 class="text-4xl sm:text-5xl lg:text-6xl font-display text-stone-900 tracking-tight">
                    당신의 삶을 재건축하는<br>12가지 거룩한 청사진
                </h1>
                <p class="mt-6 max-w-2xl mx-auto text-lg sm:text-xl text-stone-600">
                    세상의 성공 공식에 지친 당신을 위해, 하나님 나라의 원리로 승리하는 킹덤 빌더의 길을 제시합니다. 지금, 당신의 위대한 여정을 시작하십시오.
                </p>
                <div class="mt-10">
                    <a href="#part1" class="bg-amber-500 text-white font-bold py-3 px-8 rounded-full text-lg hover:bg-amber-600 transition-all duration-300 shadow-lg hover:shadow-xl">
                        건축 시작하기
                    </a>
                </div>
            </div>
        </section>

        <!-- Part 1: THE FOUNDATION -->
        <section id="part1" class="py-20 sm:py-24">
            <div class="container mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center">
                    <h2 class="text-base font-bold text-amber-600 tracking-wider">PART 1. 기초 공사</h2>
                    <p class="mt-2 text-3xl sm:text-4xl font-display text-stone-800">내면의 반석을 세우다</p>
                    <p class="mt-4 max-w-2xl mx-auto text-lg text-stone-600">모든 위대한 건축은 보이지 않는 기초에서 시작됩니다. 당신의 열망과 정체성, 그리고 두려움을 다루는 법을 재설계합니다.</p>
                </div>
                <div class="mt-16 grid gap-8 md:grid-cols-3">
                    <div class="chapter-card card-hover bg-white p-8 rounded-2xl shadow-lg cursor-pointer" data-chapter="1">
                        <span class="text-amber-500 font-bold text-sm">CHAPTER 1</span>
                        <h3 class="mt-2 text-xl font-bold text-stone-800">열망의 재설계</h3>
                        <p class="mt-2 text-stone-600">세상이 주입한 욕망이 아닌, 하나님이 주신 거룩한 열망을 발견합니다.</p>
                    </div>
                    <div class="chapter-card card-hover bg-white p-8 rounded-2xl shadow-lg cursor-pointer" data-chapter="2">
                        <span class="text-amber-500 font-bold text-sm">CHAPTER 2</span>
                        <h3 class="mt-2 text-xl font-bold text-stone-800">정체성의 확립</h3>
                        <p class="mt-2 text-stone-600">성과가 아닌 은혜 위에, 흔들리지 않는 나의 진짜 정체성을 세웁니다.</p>
                    </div>
                    <div class="chapter-card card-hover bg-white p-8 rounded-2xl shadow-lg cursor-pointer" data-chapter="3">
                        <span class="text-amber-500 font-bold text-sm">CHAPTER 3</span>
                        <h3 class="mt-2 text-xl font-bold text-stone-800">멘탈 알고리즘</h3>
                        <p class="mt-2 text-stone-600">내면의 '골리앗'이라는 두려움을, 믿음으로 해킹하고 승리하는 기술을 배웁니다.</p>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- Part 2: THE BLUEPRINT -->
        <section id="part2" class="py-20 sm:py-24 bg-white">
            <div class="container mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center">
                    <h2 class="text-base font-bold text-amber-600 tracking-wider">PART 2. 설계</h2>
                    <p class="mt-2 text-3xl sm:text-4xl font-display text-stone-800">보이지 않는 것을 건축하다</p>
                    <p class="mt-4 max-w-2xl mx-auto text-lg text-stone-600">믿음은 상상이 아니라 가장 정교한 현실 설계입니다. 당신의 미래와 하루를 하나님의 원리로 설계하는 법을 배웁니다.</p>
                </div>
                <div class="mt-16 grid gap-8 md:grid-cols-3">
                    <div class="chapter-card card-hover bg-white p-8 rounded-2xl shadow-lg cursor-pointer border border-stone-200" data-chapter="4">
                        <span class="text-amber-500 font-bold text-sm">CHAPTER 4</span>
                        <h3 class="mt-2 text-xl font-bold text-stone-800">비전 캐스팅</h3>
                        <p class="mt-2 text-stone-600">나의 꿈을 넘어, 하나님의 약속을 내 삶의 청사진으로 삼는 법을 배웁니다.</p>
                    </div>
                    <div class="chapter-card card-hover bg-white p-8 rounded-2xl shadow-lg cursor-pointer border border-stone-200" data-chapter="5">
                        <span class="text-amber-500 font-bold text-sm">CHAPTER 5</span>
                        <h3 class="mt-2 text-xl font-bold text-stone-800">절대 루틴</h3>
                        <p class="mt-2 text-stone-600">의지가 아닌 시스템으로 승리합니다. 당신의 24시간을 재창조하는 영적 습관을 설치합니다.</p>
                    </div>
                    <div class="chapter-card card-hover bg-white p-8 rounded-2xl shadow-lg cursor-pointer border border-stone-200" data-chapter="6">
                        <span class="text-amber-500 font-bold text-sm">CHAPTER 6</span>
                        <h3 class="mt-2 text-xl font-bold text-stone-800">재능의 연금술</h3>
                        <p class="mt-2 text-stone-600">하나님이 주신 고유한 재능을 발견하고, 연단하여 세상에 사용하는 법을 배웁니다.</p>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- Part 3: THE ENGINE -->
        <section id="part3" class="py-20 sm:py-24">
            <div class="container mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center">
                    <h2 class="text-base font-bold text-amber-600 tracking-wider">PART 3. 엔진</h2>
                    <p class="mt-2 text-3xl sm:text-4xl font-display text-stone-800">세상을 움직이는 시스템을 구축하다</p>
                    <p class="mt-4 max-w-2xl mx-auto text-lg text-stone-600">하나님 나라의 원리는 당신의 삶에 강력한 성장 엔진을 장착합니다. 재정과 관계, 그리고 노력의 법칙을 배웁니다.</p>
                </div>
                <div class="mt-16 grid gap-8 md:grid-cols-3">
                    <div class="chapter-card card-hover bg-white p-8 rounded-2xl shadow-lg cursor-pointer" data-chapter="7">
                        <span class="text-amber-500 font-bold text-sm">CHAPTER 7</span>
                        <h3 class="mt-2 text-xl font-bold text-stone-800">머니 매트릭스</h3>
                        <p class="mt-2 text-stone-600">세상의 결핍과 소유의 굴레에서 벗어나, 공급과 청지기의 재정 원리를 배웁니다.</p>
                    </div>
                    <div class="chapter-card card-hover bg-white p-8 rounded-2xl shadow-lg cursor-pointer" data-chapter="8">
                        <span class="text-amber-500 font-bold text-sm">CHAPTER 8</span>
                        <h3 class="mt-2 text-xl font-bold text-stone-800">세 겹 줄의 법칙</h3>
                        <p class="mt-2 text-stone-600">혼자서는 위대해질 수 없습니다. 시너지를 폭발시키는 영적 동역의 비밀을 배웁니다.</p>
                    </div>
                    <div class="chapter-card card-hover bg-white p-8 rounded-2xl shadow-lg cursor-pointer" data-chapter="9">
                        <span class="text-amber-500 font-bold text-sm">CHAPTER 9</span>
                        <h3 class="mt-2 text-xl font-bold text-stone-800">인풋-아웃풋의 법칙</h3>
                        <p class="mt-2 text-stone-600">당신의 수고가 어떻게 30배, 60배, 100배의 열매로 돌아오는지에 대한 원리를 배웁니다.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Part 4: THE COMPLETION -->
        <section id="part4" class="py-20 sm:py-24 bg-white">
            <div class="container mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center">
                    <h2 class="text-base font-bold text-amber-600 tracking-wider">PART 4. 완성</h2>
                    <p class="mt-2 text-3xl sm:text-4xl font-display text-stone-800">한계를 넘어 다음 시대를 열다</p>
                    <p class="mt-4 max-w-2xl mx-auto text-lg text-stone-600">진정한 성공은 '나'를 넘어 다음 세대를 향합니다. 당신의 삶이 세상에 남길 위대한 유산을 준비하십시오.</p>
                </div>
                <div class="mt-16 grid gap-8 md:grid-cols-3">
                    <div class="chapter-card card-hover bg-white p-8 rounded-2xl shadow-lg cursor-pointer border border-stone-200" data-chapter="10">
                        <span class="text-amber-500 font-bold text-sm">CHAPTER 10</span>
                        <h3 class="mt-2 text-xl font-bold text-stone-800">역경의 레버리지</h3>
                        <p class="mt-2 text-stone-600">실패를 성공의 지렛대로 바꾸는 기술. 최악의 상황을 최고의 기회로 전환합니다.</p>
                    </div>
                    <div class="chapter-card card-hover bg-white p-8 rounded-2xl shadow-lg cursor-pointer border border-stone-200" data-chapter="11">
                        <span class="text-amber-500 font-bold text-sm">CHAPTER 11</span>
                        <h3 class="mt-2 text-xl font-bold text-stone-800">영향력의 확장</h3>
                        <p class="mt-2 text-stone-600">당신의 삶이 세상을 향한 메시지가 되게 하라. 소금과 빛으로 살아가는 법을 배웁니다.</p>
                    </div>
                    <div class="chapter-card card-hover bg-white p-8 rounded-2xl shadow-lg cursor-pointer border border-stone-200" data-chapter="12">
                        <span class="text-amber-500 font-bold text-sm">CHAPTER 12</span>
                        <h3 class="mt-2 text-xl font-bold text-stone-800">영원의 관점</h3>
                        <p class="mt-2 text-stone-600">유한한 삶으로 영원한 유산을 남기는 법. 당신의 삶이 남길 마지막 질문에 답합니다.</p>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <footer class="bg-stone-800 text-white">
        <div class="container mx-auto py-12 px-4 sm:px-6 lg:px-8 text-center">
            <p class="text-2xl font-display">킹덤 빌더 | KINGDOM BUILDER</p>
            <p class="mt-4 text-stone-400">당신의 삶으로 하나님 나라를 증명하십시오.</p>
            <p class="mt-8 text-sm text-stone-500">&copy; 2025 Kingdom Builder Project. All Rights Reserved.</p>
        </div>
    </footer>

    <div id="modal" class="modal-backdrop fixed inset-0 bg-black bg-opacity-70 z-50 flex items-center justify-center p-4 opacity-0 pointer-events-none">
        <div id="modal-content" class="modal-content bg-white rounded-2xl shadow-2xl w-full max-w-2xl max-h-[90vh] overflow-y-auto p-6 sm:p-8 relative transform scale-95">
            <button id="modal-close" class="absolute top-4 right-4 text-stone-500 hover:text-stone-800 text-3xl leading-none">&times;</button>
            <div id="modal-body"></div>
        </div>
    </div>

    <script>
        const chapterData = {
            '1': { title: '1장: 열망의 재설계', content: '세상이 주입하는 ‘모방 욕망’의 실체를 파악하고, 하나님을 기뻐하는 ‘거룩한 열망’으로 당신의 마음을 재설계합니다. 킹덤 빌더의 모든 건축은 이 기초 공사에서 시작됩니다.' },
            '2': { title: '2장: 정체성의 확립', content: '세상이 주는 ‘성과 기반’ 이름표를 떼어내고, 하나님이 은혜로 주시는 ‘선언적 정체성’ 위에 당신의 삶을 세웁니다. 당신의 가치는 성과가 아닌 존재에 있습니다.' },
            '3': { title: '3장: 멘탈 알고리즘', content: '실패와 비판에 대한 두려움이라는 내면의 ‘골리앗’을 마주합니다. 문제보다 크신 하나님을 신뢰하는 ‘믿음의 알고리즘’으로 두려움을 해킹하고 승리하는 법을 배웁니다.' },
            '4': { title: '4장: 비전 캐스팅', content: '‘나의 성공’을 위한 비전이 아닌, ‘하나님의 이야기’에 동참하는 비전을 세웁니다. 보이지 않는 하나님의 약속을 당신 삶의 구체적인 청사진으로 만드는 법을 훈련합니다.' },
            '5': { title: '5장: 절대 루틴', content: '변덕스러운 의지력이 아닌, 거룩한 시스템의 힘을 신뢰합니다. 당신의 24시간을 하나님의 때(카이로스)를 위한 준비의 시간(크로노스)으로 재창조하는 영적 습관을 설치합니다.' },
            '6': { title: '6장: 재능의 연금술', content: '하나님이 주신 고유한 재능(달란트)을 발견하고, 광야의 시간 속에서 연단하며, 공동체를 세우는 거룩한 도구로 사용하는 청지기의 삶을 배웁니다.' },
            '7': { title: '7장: 머니 매트릭스', content: '세상의 ‘결핍과 소유’라는 재정 매트릭스에서 탈출합니다. 하나님의 ‘공급과 청지기’ 원리를 통해, 당신의 재정을 하나님 나라를 위한 축복의 파이프라인으로 전환합니다.' },
            '8': { title: '8장: 세 겹 줄의 법칙', content: '혼자서는 위대해질 수 없습니다. 세상의 파트너십을 넘어, 하나님을 중심으로 묶인 ‘세 겹 줄’ 동역을 통해 시너지를 폭발시키고 함께 성장하는 비밀을 배웁니다.' },
            '9': { title: '9장: 인풋-아웃풋의 법칙', content: '세상의 불공평한 보상 법칙을 넘어, “심는 대로 거두리라”는 하나님 나라의 신실한 원리를 신뢰합니다. 당신의 모든 수고가 어떻게 100배의 열매로 돌아오는지 배웁니다.' },
            '10': { title: '10장: 역경의 레버리지', content: '실패를 ‘끝’이 아닌 ‘기회’로 재정의합니다. 당신의 가장 깊은 상처와 약점이 어떻게 당신을 더 강하게 만들고, 다른 사람을 살리는 강력한 지렛대가 되는지를 배웁니다.' },
            '11': { title: '11장: 영향력의 확장', content: '세상의 ‘인플루언서’가 아닌, 하나님 나라의 ‘소금과 빛’이 되는 법을 배웁니다. 당신의 삶 전체가 당신의 말이 아닌, 당신의 ‘착한 행실’을 통해 세상을 변화시키는 메시지가 되게 합니다.' },
            '12': { title: '12장: 영원의 관점', content: '유한한 삶으로 영원한 유산을 남기는 법을 배웁니다. 이 땅의 모든 수고의 궁극적인 목적지를 확인하고, “잘하였도다 착하고 충성된 종아” 칭찬받는 삶을 향한 위대한 여정을 시작합니다.' }
        };

        document.addEventListener('DOMContentLoaded', () => {
            const modal = document.getElementById('modal');
            const modalContent = document.getElementById('modal-content');
            const modalBody = document.getElementById('modal-body');
            const modalCloseBtn = document.getElementById('modal-close');
            const chapterCards = document.querySelectorAll('.chapter-card');

            function openModal(chapterId) {
                const data = chapterData[chapterId];
                if (!data) return;

                modalBody.innerHTML = `
                    <h2 class="text-3xl font-display text-stone-800 mb-4">${data.title}</h2>
                    <p class="text-lg text-stone-600 leading-relaxed">${data.content}</p>
                `;
                
                modal.classList.remove('opacity-0', 'pointer-events-none');
                modalContent.classList.remove('scale-95');
                document.body.style.overflow = 'hidden';
            }

            function closeModal() {
                modal.classList.add('opacity-0', 'pointer-events-none');
                modalContent.classList.add('scale-95');
                document.body.style.overflow = '';
            }

            chapterCards.forEach(card => {
                card.addEventListener('click', () => openModal(card.dataset.chapter));
            });

            modalCloseBtn.addEventListener('click', closeModal);
            modal.addEventListener('click', (e) => {
                if (e.target === modal) closeModal();
            });
            document.addEventListener('keydown', (e) => {
                if (e.key === 'Escape') closeModal();
            });
        });
    </script>
</body>
</html>
