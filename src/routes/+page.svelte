<script>
    import logo from '$lib/assets/logo.svg';
    import {CodeBlock} from '@skeletonlabs/skeleton';
    import hljs from 'highlight.js/lib/core';
    import typescript from 'highlight.js/lib/languages/typescript';

    hljs.registerLanguage('typescript', typescript);
    import {storeHighlightJs} from '@skeletonlabs/skeleton';

    storeHighlightJs.set(hljs);
    import 'highlight.js/styles/base16/dracula.min.css';
</script>


<div class="relative bg-white px-6 pt-10 pb-8 shadow-xl ring-1 ring-gray-900/5 sm:mx-auto sm:max-w-2xl sm:rounded-2xl sm:px-10">
    <div class="mx-auto max-w-2xl">
        <img src={logo} class="h-6" alt="Tailwind Play"/>
        <div class="divide-y divide-gray-300/50">
            <div class="space-y-6 py-8 text-base leading-7 text-gray-600">
                <p>다음과 같은 기능을 지원하는 Tailwind CSS용 고급 온라인 플레이그라운드입니다.</p>
                <CodeBlock class="bg-[#282936]" lineNumbers language="ts" code={`import hljs from 'highlight.js/lib/core';

// Import each language module you require
import xml from 'highlight.js/lib/languages/xml'; // for HTML
import css from 'highlight.js/lib/languages/css';
import json from 'highlight.js/lib/languages/json';
import javascript from 'highlight.js/lib/languages/javascript';
import typescript from 'highlight.js/lib/languages/typescript';
import shell from 'highlight.js/lib/languages/shell';

// Register each imported language module
hljs.registerLanguage('xml', xml); // for HTML
hljs.registerLanguage('css', css);
hljs.registerLanguage('json', json);
hljs.registerLanguage('javascript', javascript);
hljs.registerLanguage('typescript', typescript);
hljs.registerLanguage('shell', shell);`}></CodeBlock>
                <ul class="space-y-4">
                    <li class="flex items-center">
                        <svg class="h-6 w-6 flex-none fill-sky-100 stroke-sky-500 stroke-2" stroke-linecap="round"
                             stroke-linejoin="round">
                            <circle cx="12" cy="12" r="11"/>
                            <path d="m8 13 2.165 2.165a1 1 0 0 0 1.521-.126L16 9" fill="none"/>
                        </svg>
                        <p class="ml-4">
                            <code class="text-sm font-bold text-gray-900">tailwind.config.js</code> 파일 사용자 정의
                        </p>
                    </li>
                    <li class="flex items-center">
                        <svg class="h-6 w-6 flex-none fill-sky-100 stroke-sky-500 stroke-2" stroke-linecap="round"
                             stroke-linejoin="round">
                            <circle cx="12" cy="12" r="11"/>
                            <path d="m8 13 2.165 2.165a1 1 0 0 0 1.521-.126L16 9" fill="none"/>
                        </svg>
                        <p class="ml-4">
                            <code class="text-sm font-bold text-gray-900">@apply</code> 클래스 추출
                        </p>
                    </li>
                    <li class="flex items-center">
                        <svg class="h-6 w-6 flex-none fill-sky-100 stroke-sky-500 stroke-2" stroke-linecap="round"
                             stroke-linejoin="round">
                            <circle cx="12" cy="12" r="11"/>
                            <path d="m8 13 2.165 2.165a1 1 0 0 0 1.521-.126L16 9" fill="none"/>
                        </svg>
                        <p class="ml-4">즉시 미리보기로 코드 완성</p>
                    </li>
                </ul>
                <p>프레임워크 작동 방식을 배우고, 새로운 아이디어의 프로토타입을 제작하거나, 온라인으로 공유할 데모를 만드는 데 적합합니다.</p>
            </div>
            <div class="pt-8 text-base font-semibold leading-7">
                <p class="text-gray-900">Tailwind에 대해 더 자세히 알아보고 싶으신가요?</p>
                <p>
                    <a href="https://tailwindcss.com/docs" class="text-sky-500 hover:text-sky-600">상세정보
                        &rarr;</a>
                </p>
            </div>
        </div>
    </div>
</div>