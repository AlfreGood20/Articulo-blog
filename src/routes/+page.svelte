<script>
    let abierto = false;
</script>

<nav class="w-full p-2 md:p-0 shadow-lg font-bold">

    <button class="md:hidden p-2 cursor-pointer" on:click={() => (abierto = !abierto)} aria-label="Abrir menú">
        
        <svg class="w-8 h-8" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                d="M4 6h16M4 12h16M4 18h16" />
        </svg>
    </button>

    <ul class={`flex-col md:flex-row gap-3 md:gap-6 p-2 md:p-4 justify-center w-full font-bold bg-white ${abierto ? 'flex' : 'hidden'} md:flex`}>
        <li>
            <a href="#inicio" class="p-2 hover:bg-gray-200 rounded">Inicio</a>
        </li>
        <hr class="border-green-600">
        <li>
            <a href="#" class=" p-2 hover:bg-gray-200 rounded">Concepto</a>
        </li>
        <hr class="border-amber-300">
        <li>
            <a href="#" class=" p-2 hover:bg-gray-200 rounded">Objetivos</a>
        </li>
        <hr class="border-blue-600">
        <li>
            <a href="#" class=" p-2 hover:bg-gray-200 rounded">Usos</a>
        </li>
        <hr class="border-cyan-400">
        <li>
            <a href="#" class=" p-2 hover:bg-gray-200 rounded">Arquitectura de una bd</a>
        </li>
        <hr class="border-orange-900">
        <li>
            <a href="#" class=" p-2 hover:bg-gray-200 rounded">Arquitectura del SGBD</a>
        </li>
        <hr>
    </ul>
</nav>

<!--NOTAS Y INFORMCION-->
<div class="flex-1 md:flex gap-6 flex-row md:h-[530px]">

    <section class="flex-1 md:h-130 bg-white shadow-md m-2 md:mt-5 md:ml-6 rounded border border-gray-300 font-['Times_New_Roman'] overflow-y-auto">

        <div class="flex flex-col">
            <h1 id="inicio" class="m-3 font-extrabold text-4xl">Bases de datos</h1>
            <p class="ml-3 mb-2 text-sm">27 de enero de 2026</p>
            <div class="flex justify-center">
                <img src="/imgs/ilustracion.jpg" alt="Ilustración de bases de datos" class="w-xs  md:w-2xl md:h-60 rounded md:mx-10"/>
            </div>

            <div class="animate-pulse p-2 mt-2 mx-3">
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
            </div>

            <div class="animate-pulse p-2 mt-2 mx-3">
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
            </div>

            <div class="animate-pulse p-2 mt-2 mx-3">
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
            </div>

            <div class="animate-pulse p-2 mt-2 mx-3">
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
            </div>

            <div class="animate-pulse p-2 mt-2 mx-3">
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
            </div>

            <div class="animate-pulse p-2 mt-2 mx-3">
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
            </div>

            <div class="animate-pulse p-2 mt-2 mx-3">
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
            </div>

            <div id="example" class="animate-pulse p-2 mt-2 mx-3">
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
            </div>
        </div>
    </section>

     <section class="m-2 md:w-60 md:h-130 bg-white shadow-md md:mt-5 md:mr-5 rounded border border-gray-300 font-['Times_New_Roman']">

        <h2 class="mt-3 ml-3 font-semibold text-lg">Universidad</h2>
        <div class="flex flex-col items-center justify-center">
            <img src="/imgs/ITVH.jpg" alt="Logo del instituto" class="w-20 h-20 rounded mb-2"/>
            <a class="text-center" href="https://villahermosa.tecnm.mx/">Instituto Tecnológico de Villahermosa</a>
        </div>
        <hr class="my-2 mx-4 border-gray-300">

        <h2 class="mt-2 ml-3 font-semibold text-lg">Autores</h2>
        <ul>
            <li class="m-3 text-sm">
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
            </li>
            <li class="m-3 text-sm">
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
            </li>
            <li class="m-3 text-sm">
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
            </li>
            <li class="m-3 text-sm">
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
            </li>
            <li class="m-3 text-sm">
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
            </li>
        </ul>
        <hr class="my-2 mx-4  border-gray-300">

        <h2 class="mt-2 ml-3 font-semibold text-lg">Correos</h2>
        <ul>
            <li class="m-3 text-sm">
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
            </li>
            <li class="m-3 text-sm">
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
            </li>
            <li class="m-3 text-sm">
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
            </li>
            <li class="m-3 text-sm">
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
            </li>
            <li class="m-3 text-sm">
                <div class="h-3 bg-slate-700 rounded w-full mb-1"></div>
            </li>
        </ul>
    </section>
</div>

<footer class="w-full mt-3 md:p-4 bg-gradient-to-r from-neutral-600 to-neutral-500 text-white text-center md:mt-5">
    &copy; 2026 Hecho por estudiantes del ITVH. Todos los derechos reservados.
</footer>