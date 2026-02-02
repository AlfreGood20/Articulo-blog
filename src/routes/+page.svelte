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
            <a href="#concepto" class=" p-2 hover:bg-gray-200 rounded">Concepto</a>
        </li>
        <hr class="border-amber-300">
        <li>
            <a href="#objetivos" class=" p-2 hover:bg-gray-200 rounded">Objetivos</a>
        </li>
        <hr class="border-blue-600">
        <li>
            <a href="#usos" class=" p-2 hover:bg-gray-200 rounded">Usos</a>
        </li>
        <hr class="border-cyan-400">
        <li>
            <a href="#artBD" class=" p-2 hover:bg-gray-200 rounded">Arquitectura de una bd</a>
        </li>
        <hr class="border-orange-900">
        <li>
            <a href="#artSGBD" class=" p-2 hover:bg-gray-200 rounded">Arquitectura del SGBD</a>
        </li>
        <hr>
        <li>
            <a href='#' on:click={() => alert("PROXIMAMENTE MAS INFORMACIÓN")}  class=" p-2 hover:bg-gray-200 rounded">Más información</a>
        </li>
    </ul>
</nav>

<!--NOTAS Y INFORMCION-->
<div class="flex-1 md:flex gap-6 flex-row md:h-[530px]">

    <section class="flex-1 md:h-130 bg-white shadow-md m-2 md:mt-5 md:ml-6 rounded border border-gray-300 font-['Times_New_Roman'] overflow-y-auto">

        <div class="flex flex-col">
            <h1 id="inicio" class="m-3 font-extrabold text-4xl">Arquitectura de Bases de Datos y SGBD</h1>
            <p class="ml-3 mb-2 text-sm">03 De Febrero De 2026</p>
            <div class="flex justify-center">
                <img src="/imgs/ilustracion.jpg" alt="Ilustración de bases de datos" class="w-xs  md:w-2xl md:h-60 rounded md:mx-10"/>
            </div>

            <div class="m-3 text-justify">

                <p>
                    Las bases de datos son el pilar fundamental de los sistemas de información
                    modernos. Para garantizar un manejo eficiente, seguro y flexible de los datos,
                    se utiliza una arquitectura de base de datos, la cual define cómo se organiza la
                    información y cómo interactúan los usuarios y las aplicaciones con ella.
                    Esta arquitectura permite separar los distintos niveles de manejo de los datos,
                    logrando independencia, seguridad y facilidad de mantenimiento.
                </p>

                <h3 id="concepto" class="font-bold text-lg mt-4">¿Qué es una base de datos?</h3>
                <p>
                    Una base de datos es una colección estructurada de datos. Se almacena y
                    organiza para facilitar su recuperación, manipulación y actualización. 
                </p>
                <p>Proporciona una forma sistemática de acceder, gestionar y actualizar la información.</p>

                <p class="mt-2">Se compone de tres componentes principales:</p>
                <ol class="list-decimal ml-6">
                    <li>Los datos en sí.</li>
                    <li>El sistema de gestión de bases de datos (SGBD) que facilita el acceso y la manipulación de los datos</li>
                    <li>La aplicación de base de datos que sirve como interfaz entre los usuarios y la base de datos.</li>
                </ol>

                <h3 id="objetivos" class="font-bold text-lg mt-4">Objetivos</h3>

                <div class="grid grid-cols-1 md:grid-cols-2 gap-4 mt-2">

                    <div class="bg-white shadow-lg flex flex-col justify-center items-center p-5 animate hover:-translate-y-1 hover:shadow-2xl transition-all duration-300">
                        <h3 class="text-center font-bold">Almacenamiento de información de forma estructurada</h3>
                        <img src="/imgs/PRIMER OBJETIVO.jpg" class="w-50 h-50 mx-auto" alt="ilustracion">
                        <p>
                            En un SGDB (Sistema De Gestión De Bases De Datos ) es fundamental organizar los datos
                            eficientemente, permitir consultas rápidas, mantener la integridad de la información y facilitar su
                            administración.
                        </p>
                    </div>

                    <div class="bg-white shadow-lg flex flex-col justify-center items-center p-5 animate hover:-translate-y-1 hover:shadow-2xl transition-all duration-300">
                        <h3 class="text-center font-bold">Integridad y precisión de los datos</h3>
                        <img src="/imgs/SEGUNDO OBJETIVO.jpg" class="w-50 h-50 mx-auto" alt="ilustracion">
                        <p>
                            La integridad de los datos se refiere a la precisión y consistencia de los datos a lo largo de su ciclo de
                            vida. Un SGBD aplica las reglas y restricciones definidas en el esquema de la base de datos para
                            garantizar que solo se ingresen y mantengan datos precisos.
                        </p>
                    </div>

                    <div class="bg-white shadow-lg flex flex-col justify-center items-center p-5 animate hover:-translate-y-1 hover:shadow-2xl transition-all duration-300">
                        <h3 class="text-center font-bold">Seguridad de datos</h3>
                        <img src="/imgs/TERCER OBJETIVO.jpg" class="w-50 h-50 mx-auto" alt="ilustracion">
                        <p>
                            Un SGBD proporciona mecanismos de seguridad robustos, que incluyen cifrado, control de acceso de
                            usuarios y autenticación, para proteger contra el acceso no autorizado.
                        </p>
                    </div>

                    <div class="bg-white shadow-lg flex flex-col justify-center items-center p-5 animate hover:-translate-y-1 hover:shadow-2xl transition-all duration-300">
                        <h3 class="text-center font-bold">Garantizar una alta independencia de los datos</h3>
                        <img src="/imgs/CUARTO OBJETIVO.jpg" class="w-50 h-50 mx-auto rounded-2xl" alt="ilustracion">
                        <p>
                            La independencia de datos se refiere a la capacidad de cambiar el esquema (la estructura de la base
                            de datos) sin afectar a los datos en sí.
                        </p>
                    </div>

                </div>

                <h3 id="usos" class="font-bold mt-5 text-lg">Ejemplo de usos:</h3>
                <ol class="list-disc ml-6">
                    <li>
                        <p class="font-bold">Transacciones bancarias y financieras: </p>
                        <p>Los bancos utilizan bases de datos para almacenar información de las cuentas de sus clientes, historiales de transacciones y saldos</p>
                    </li>
                    <li>
                        <p class="font-bold"> Compras en línea: </p>
                        <p>Las plataformas de comercio electrónico se basan en bases de datos para almacenar catálogos de productos, pedidos de clientes y niveles de inventario.</p>
                    </li>
                    <li>
                        <p class="font-bold">Plataformas de redes sociales: </p>
                        <p>Las redes sociales utilizan bases de datos para almacenar perfiles de usuarios, publicaciones, comentarios y "me gusta".</p>
                    </li>
                </ol>

                <h3 id="artBD" class="font-bold mt-5 text-lg">Niveles de la arquitectura de una base de datos</h3>
                <p>La arquitectura de bases de datos se organiza en tres niveles, conocidos como la arquitectura de tres esquemas (ANSI/SPARC):</p>

                <h3 class="font-bold mt-4">1.Nivel Externo o de Vistas</h3>
                <p class="underline">Es el nivel más cercano a los usuarios finales</p>

                 <ol class="list-disc ml-6">
                    <li>Representa la forma en que los usuarios o aplicaciones ven los datos.</li>
                    <li>Cada usuario puede tener una vista distinta de la base de datos.</li>
                    <li>No muestra toda la información, solo la necesaria.</li>
                </ol>
                
                <p class="text-center">Una manera de comprenderlo desde el un aspecto de la vida diaria seria el siguiente ejemplo: 
                    <br>Un empleado solo puede ver sus datos personales, no los de otros empleados.
                </p>

                <h3 class="font-bold mt-5 text-lg">2. Nivel Conceptual o Lógico</h3>
                <p class="underline">Define la estructura lógica de toda la base de datos para la comunidad de usuarios.</p>
                <ol class="list-disc ml-6">
                    <li>Describe la estructura lógica completa de la base de datos.</li>
                    <li>Define tablas, relaciones, atributos y restricciones.</li>
                    <li>Es independiente de cómo se almacenan los datos físicamente.</li>
                </ol>
                <p class="text-center">En relación a esto se puede tomar como ejemplo lo siguiente, con relación a este nivel:
                    <br>El establecer que existe una tabla Clientes relacionada con Pedidos.
                </p>

                <h3 class="font-bold mt-5 text-lg">3. Nivel Interno o Físico:</h3>
                <p class="underline">Describe cómo se almacenan físicamente los datos en el hardware. Se encarga de la organización de archivos, índices y estructuras de almacenamiento.</p>
                <ol class="list-disc ml-6">
                    <li>Define cómo se almacenan los datos en el sistema.</li>
                    <li>Incluye archivos, índices, métodos de acceso y almacenamiento.</li>
                    <li>Está relacionado directamente con el hardware.</li>
                </ol>
                <p class="text-center">Para lograr entender mejor este nivel, un ejemplo para demostrar lo que este hace, es lo siguiente:
                    <br>Cuando se guardan los registros en disco duro o SSD, para conservar la información.
                </p>

                <h3 class="font-bold mt-5 text-lg">La independencia de datos permite modificar un nivel sin afectar a los demás.</h3>
                <ol class="list-disc ml-6">
                    <li>
                        <p class="font-bold">Independencia física</p>
                        <ol class="list-disc ml-5">
                            <li>Cambios en el nivel interno no afectan al nivel conceptual ni externo.</li>
                            <li>Ejemplo: cambiar el tipo de almacenamiento sin modificar las tablas</li>
                        </ol>
                    </li>

                    <li>
                        <p class="font-bold">Independencia lógica</p>
                        <ol class="list-disc ml-5">
                            <li>Cambios en el nivel conceptual no afectan las vistas externas.</li>
                            <li>Ejemplo: agregar un campo nuevo a una tabla sin afectar a los usuarios.</li>
                        </ol>
                    </li>
                </ol>

                <p class="text-center underline font-bold mt-2">La importancia de esta interdependencia de datos está en que permite que los sistemas sean más flexibles, escalables y fáciles de mantener.</p>

                <h3 id="artSGBD" class="font-bold mt-5 text-lg">Arquitectura de un SGBD (Sistema Gestor de Bases de Datos)</h3>
                <div class="flex justify-center mt-2">
                    <img src="/imgs/SGBD ILUSTRACION.png" alt="Ilustración SGBD" class="w-xs  md:w-2xl md:h-60 rounded md:mx-10"/>
                </div>

                <p class="text-center">
                    Un SGBD consta de varios componentes, cada uno de los cuales realiza tareas muy
                    importantes en el entorno del sistema de gestión de bases de datos:
                </p>

                <p class="mt-2 font-bold">Componentes del SGBD</p>
                <p class="mt-5">1. Motor de Base de Datos</p>
                <p>El servicio principal para almacenar, procesar y proteger datos proporciona acceso controlado y un procesamiento rápido de transacciones para satisfacer las necesidades de las aplicaciones más exigentes que consumen datos.</p>

                <p class="mt-5">2. Gestor de Almacenamiento</p>
                <p>Maneja la lectura y escritura de datos en disco y memoria.</p>

                <p class="mt-5">3. Procesador de Consultas</p>
                <p>
                    Este transforma las consultas del usuario en una serie de instrucciones de bajo nivel. Lee la
                    consulta del usuario en línea o dentro del sistema y la traduce en una serie eficiente de
                    operaciones, capaces de enviarse al gestor de datos en tiempo de ejecución para su
                    ejecución.
                </p>

                <p class="mt-5">4. Diccionario de Datos</p>
                <p>Almacena información sobre la estructura de la base de datos</p>

                <p class="mt-5">5. Gestor de Transacciones</p>
                <p>Asegura la integridad y consistencia (ACID) de las operaciones, controlando la concurrencia.</p>

                <p class="mt-5">6. Gestor de Seguridad</p>
                <p>
                    Es el conjunto de componentes y mecanismos, como el DCL (Data Control Language),
                    cifrado, y control de acceso (autenticación/autorización), que protegen la información
                    contra accesos no autorizados, integridad comprometida o fallos accidentales.
                </p>

                <p class="mt-5">7. Software</p>
                <p>
                    Es el conjunto de programas utilizados para controlar y gestionar la base de datos en su
                    conjunto. Incluye el propio software del SGBD, el sistema operativo, el software de red
                    utilizado para compartir los datos entre los usuarios y las aplicaciones utilizadas para
                    acceder a los datos del SGBD.
                </p>

                <p class="mt-5">8. Hardware</p>
                <p>
                    Consiste en un conjunto de dispositivos electrónicos físicos como computadoras,
                    dispositivos de E/S, dispositivos de almacenamiento, etc., esto proporciona la interfaz
                    entre las computadoras y los sistemas del mundo real.
                </p>

                <h3 class="font-bold mt-5 text-lg">Importancia de la arquitectura del SGBD</h3>
                <ol class="ml-6 list-disc">
                    <li>
                        Permite organizar eficientemente la información.
                    </li>

                    <li>
                        Mejora la seguridad y consistencia de los datos.
                    </li>

                    <li>
                        Facilita el mantenimiento y evolución del sistema.
                    </li>

                    <li>
                        Facilita el mantenimiento y evolución del sistema.
                    </li>

                    <li>
                        Garantiza el acceso simultáneo de múltiples usuarios.
                    </li>
                </ol>

                <h3 class="font-bold text-lg mt-8">Fuentes Bibliograficas</h3>
                <ul class="list-disc ml-6 mt-2 text-sm">
                    <li>
                        Components of a database management system. (s/f). Dataentryoutsourced.com. Recuperado el 2 de febrero de 2026, de 
                        <a href="https://www.dataentryoutsourced.com/blog/components-of-a-databasemanagement-system/" class="text-blue-600 underline" target="_blank">https://www.dataentryoutsourced.com/blog/components-of-a-databasemanagement-system/</a>
                    </li>
                    <li>
                        Components of DBMS (database management system). (2023, mayo 5). InterviewBit. 
                        <a href="https://www.interviewbit.com/blog/components-of-dbms/" class="text-blue-600 underline" target="_blank">https://www.interviewbit.com/blog/components-of-dbms/</a>
                    </li>
                    <li>
                        GeeksforGeeks. (2025, 9 October). DBMS architecture 1-level, 2-level, 3-level. GeeksforGeeks. 
                        <a href="https://www.geeksforgeeks.org/dbms-architecture-2-level-3-level/" class="text-blue-600 underline" target="_blank">https://www.geeksforgeeks.org/dbms-architecture-2-level-3-level/</a>
                    </li>
                    <li>
                        TutorialsPoint. (2026). DBMS – Architecture. TutorialsPoint. 
                        <a href="https://www.tutorialspoint.com/dbms/dbms_architecture.htm" class="text-blue-600 underline" target="_blank">https://www.tutorialspoint.com/dbms/dbms_architecture.htm</a>
                    </li>
                    <li>
                        IBM. (n.d.). Db2 architecture and process overview. IBM Documentation. 
                        <a href="https://www.ibm.com/docs/en/db2/11.5.x?topic=architecture-db2-process-overview" class="text-blue-600 underline" target="_blank">https://www.ibm.com/docs/en/db2/11.5.x?topic=architecture-db2-process-overview</a>
                    </li>
                    <li>
                        Oracle. (2020, 24 November). What is a database? Oracle. 
                        <a href="https://www.oracle.com/database/what-is-database/" class="text-blue-600 underline" target="_blank">https://www.oracle.com/database/what-is-database/</a>
                    </li>
                    <li>
                        Elsevier. (n.d.). Database Management System. ScienceDirect. 
                        <a href="https://www.sciencedirect.com/topics/computer-science/database-management-system" class="text-blue-600 underline" target="_blank">https://www.sciencedirect.com/topics/computer-science/database-management-system</a>
                    </li>
                    <li>
                        Database Systems: Design, Implementation, and Management – libro completo en PDF (temas de diseño e implementación de sistemas de bases de datos). 
                        <a href="https://pdfroom.com/books/database-systems-design-implementation-and-management-eighthedition/zydD8bP4d14" class="text-blue-600 underline" target="_blank">https://pdfroom.com/books/database-systems-design-implementation-and-management-eighthedition/zydD8bP4d14</a>
                    </li>
                </ul>   
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
                <label for="lider">López De La Cruz José Alfredo</label>
            </li>
            <li class="m-3 text-sm">
                <label for="lider">Silvan Suarez Omar</label>
            </li>
            <li class="m-3 text-sm">
                <label for="lider">Alfonso De La Cruz Emily</label>
            </li>
            <li class="m-3 text-sm">
                <label for="lider">Lanestosa Gómez Fernado</label>
            </li>
            <li class="m-3 text-sm">
                <label for="lider">Velázquez Izquierdo Misael</label>
            </li>
        </ul>
        <hr class="my-2 mx-4  border-gray-300">

        <h2 class="mt-2 ml-3 font-semibold text-lg">Correos</h2>
        <ul>
            <li class="m-3 text-sm">
                <p>L24300777@villahermosa.tecnm.mx</p>
            </li>
            <li class="m-3 text-sm">
                <p></p>
            </li>
            <li class="m-3 text-sm">
                <p></p>
            </li>
            <li class="m-3 text-sm">
                <p></p>
            </li>
            <li class="m-3 text-sm">
                <p></p>
            </li>
        </ul>
    </section>
</div>