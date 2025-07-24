
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset='utf-8'>
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Open+Sans:300,400,600,700|Roboto:100,300,400,500,700">

    <title>Ministerio de Educación de la República Dominicana</title>

    <link rel="shortcut icon" href="img/favicon/favicon.ico" type="image/x-icon">
    <link rel="icon" href="img/favicon/favicon.ico" type="image/x-icon">

    <link href="/Content/css?v=oaYjsFbHdx4MC3fjA19ze6DB3_IOs5a3SWKupk6L9zU1" rel="stylesheet"/>

    <script src="/bundles/modernizr?v=wBEWDufH_8Md-Pbioxomt90vm6tJN2Pyy9u9zHtWsPo1"></script>

    
    <link type="text/css" href="/Content/home.css" rel="stylesheet" />

    <style type="text/css">
        .borderless td, .borderless th {
            border: none !important;
        }
    </style>

    <script>
        var ruta = window.location.origin + '/'
    </script>
</head>
<body>
    <input type="hidden" name="parentURL" value="English">
    <div id="GifContainer" class="hidden"></div>
    <div id="header" class="boxid_ header hidden-print"></div>
    <!-- FIN -->

    <div class="container body">

        <div class="col-lg-12 col-md-12 col-sm-12 col-xs-12">
            


<br />

<div class="row">
    <div class="col-md-2"></div>
    <div class="col-sm-12 col-md-12 col-lg-8" id="panel-opciones">
        <div class="panel panel-primary hidden-print">
            <div class="ph-provisional panel-heading">
                <h1 class="panel-title text-center">
                    <b>Certificación de Estudios</b>
                </h1>
            </div>
            <div class="panel-body" style="background-color: #ece9e9;">
                <div class="pb-row">
                    <div id="nvlbasico" class="col-md-12 col-lg-12 col-xs-12 col-sm-12 nvl-opcion">
                        Nivel Básico
                    </div>
                    <div id="nvlmedio" class="col-md-12 col-lg-12 col-xs-12 col-sm-12 nvl-opcion">
                        Nivel Medio/Secundario
                    </div>
                </div>
            </div>
        </div>
    </div>

    <div style="display: none;" id="panel-datos" class="col-sm-12 col-md-12 col-lg-8">
        <div class="panel panel-primary hidden-print">
            <div class="panel-heading">
                <h1 class="panel-title text-center">
                    <b style="display: none;" id="titleProvisional">Consulta Resultados Certificación Provisional</b>
                    <b style="display: none;" id="titleBasico">Certificado Nivel Básico</b>
                    <b style="display: none;" id="titleMedio">Certificado Nivel Medio/Secundario</b>
                </h1>
                
            </div>
            <div class="panel-body" style="background-color: #F7F7F7;">

                <form id="formulario">
                    <label for="busPeriCodigo">
                        Año Escolar
                    </label>
                    <div class="input-group input-group-lg">
                        <span class="input-group-addon">
                            <span class="glyphicon glyphicon-calendar"></span>
                        </span>
                        <select style="display: none;" id="drpPeriodoEscolar" class="form-control" title="Elige el año escolar"></select>
                        <select style="display: none;" id="drpPeriodoEscolarProvisional" disabled class="form-control" title="Elige el año escolar">
                            <option value="2020">PERIODO 2020</option>
                        </select>
                    </div>
                    <div id="Convocatoria" style="display: none;">
                        <label for="busConvCodigo">
                            Convocatoria
                        </label>
                        <div class="input-group input-group-lg">
                            <span class="input-group-addon">
                                <span class="glyphicon glyphicon-pencil"></span>
                            </span>
                            <select id="drpConvocatorias" class="form-control" title="Elige la convocatoria"></select>
                        </div>
                    </div>
                    <div id="TipoEstudio" style="display: none;">
                        <label for="TipoEstudioLbl">
                            Tipo de Estudio
                        </label>
                        <div class="input-group input-group-lg">
                            <span class="input-group-addon">
                                <span class="glyphicon glyphicon-pencil"></span>
                            </span>
                            <select id="drpTipoEstudios" class="form-control" title="Elige el tipo de estudio">
                                    <option value="Conclusi&#243;n de Estudios Medio">Conclusi&#243;n de Estudios Medio</option>
                            </select>
                        </div>
                    </div>
                    <label for="busMrneCodigo">
                        Código de Estudiante (RNE o NUMERO DE REGISTRO)
                    </label>
                    <div class="input-group input-group-lg">
                        <span class="input-group-addon"><span class="glyphicon glyphicon-user"></span></span>
                        <input class="form-control" data-val="true" data-val-required="Este campo es obligatorio" id="txtRNE" name="RNE" placeholder="RNE" title="Ingresa el Registro Nacional de Estudiante (RNE)" type="text" value="" />
                        
                    </div>


                    <div style="color:red;">
                        <span class="field-validation-valid" data-valmsg-for="RNE" data-valmsg-replace="true"></span>
                    </div>

                    <br />

                    <div align="center">



                            <div class="g-recaptcha" data-sitekey="6Le2ZCUUAAAAADKjdiDfuRfh-TKgfjd2uxGvLmEy"></div>

                        <input type="button" id="btnBuscar" class="btn btn-primary btn-lg" tooltip="Buscar Información según Criterios" value="Buscar" />

                        <br />
                        <br />

                        
                        <a id="aRNE" style="margin: 10px 0">
                            <span style="color: #21374c; font-size:18px;">Obtener mi RNE</span>
                        </a>
                    </div>
                </form>
            </div>
        </div>
        <div>
            <button id="btn-volver" class="btn btn-volver col-md-12">Volver</button>
        </div>
    </div>

    <div id="resultadosBusquedaRne" style="display: none;">
        <div id="resultados">

        </div>
        <div id="resultados-footer">
            <button id="btnVolverResultado" class="btn btn-primary">
                Volver
            </button>
        </div>
    </div>
    <div class="col-sm-2"></div>
</div>

<div id="msjError" class="row hidden">
    <div id="msjOriginal" class="col-md-12 col-sm-12 col-lg-12 hidden">
        <b>IMPORTANTE:</b> Su certificado no aparece en la base de datos de Pruebas Nacionales. Si es un estudiante que concluyó entre los años 1994-2000 se requiere crear su código RNE y actualizar.
        Para ello, debe dirigirse al Distrito Educativo o la oficina de la Dirección de Evaluación de la Calidad con la copia del acta de nacimiento o cédula y la copia del acta de Pruebas Nacionales donde aparece promovido (esta acta puede estar en el centro educativo o el distrito).
        Para más información puede comunicarse al 809-687-7400 y al correo electrónico <a href="mailto:evaluaciondelacalidad@minerd.gob.do"> evaluaciondelacalidad@minerd.gob.do</a>
    </div>
</div>

<div id="msjNoDefinido" class="row hidden">


</div>



        </div>
        
    </div>




    <!-- Footer Contenedor -->
    <div id="footer" class="boxid_ footerInfo hidden-print"></div>
    <!-- Fin Footer Contenedor -->

    <script src="/bundles/jquery?v=CGonZMwpYj9-G72t0B-UwLtd5oBPn49Jo2d3GRUrSoU1"></script>

    <script src="/bundles/bootstrap?v=AcWl1dxknO7L_sfwfW4HMnBs3ckIPsEBOCvihmI2k2w1"></script>

    <script src="/bundles/Utility?v=cJSFsj8gQhxvzQyx3JoAazHaroelw47epYUM3v_-AP81"></script>

    <script src='https://www.google.com/recaptcha/api.js?hl=es'></script>
    <script type="text/javascript" src="/Scripts/root.js"></script>
    <script src="/Scripts/balloon.js"></script>

    <script language="javascript">
        /*google analytics */
        (function (i, s, o, g, r, a, m) {
            i['GoogleAnalyticsObject'] = r; i[r] = i[r] || function () {
                (i[r].q = i[r].q || []).push(arguments)
            }, i[r].l = 1 * new Date(); a = s.createElement(o),
                m = s.getElementsByTagName(o)[0]; a.async = 1; a.src = g; m.parentNode.insertBefore(a, m)
        })(window, document, 'script', '//www.google-analytics.com/analytics.js', 'ga');

        ga('create', 'UA-35956730-4', 'minerd.gob.do');
        ga('send', 'pageview');

        /*End google analytics */

        /*Application Insight */
            var appInsights=window.appInsights||function(a){
        function b(a){c[a]=function(){var b=arguments;c.queue.push(function(){c[a].apply(c,b)})}}var c={config:a},d=document,e=window;setTimeout(function(){var b=d.createElement("script");b.src=a.url||"https://az416426.vo.msecnd.net/scripts/a/ai.0.js",d.getElementsByTagName("script")[0].parentNode.appendChild(b)});try{c.cookie=d.cookie}catch(a){}c.queue=[];for(var f=["Event","Exception","Metric","PageView","Trace","Dependency"];f.length;)b("track"+f.pop());if(b("setAuthenticatedUserContext"),b("clearAuthenticatedUserContext"),b("startTrackEvent"),b("stopTrackEvent"),b("startTrackPage"),b("stopTrackPage"),b("flush"),!a.disableExceptionTracking){f="onerror",b("_"+f);var g=e[f];e[f]=function(a,b,d,e,h){var i=g&&g(a,b,d,e,h);return!0!==i&&c["_"+f](a,b,d,e,h),i}}return c
        }({
        instrumentationKey:"e03cdc85-d11e-48c2-97f3-00f72d4f0017"
        });
        window.appInsights = appInsights, appInsights.queue && 0 === appInsights.queue.length && appInsights.trackPageView();
        /* End Application Insight */

        /*Se corrige ruta de las imagenes de los logos*/
        $(document).ready(function () {
            
            $("img").each(function () {
                var source = $(this).attr("src")
                $(this).attr("src", corregirRuta(source));
                } 
            );
            $("link").each(function () {
                var source = $(this).attr("href")
                $(this).attr("href", corregirRuta(source));
                }  
            );

            function corregirRuta(root) {
                if ((root.indexOf('http') === -1 && root.indexOf('/') === -1) || (root.indexOf('http') === -1 && '/'==='/')) {
                    root = window.location.origin + ("/" + root).replace('//', '/');
                } 
                return root;
            }
        });
        
        /*Fin corrige ruta de las imagenes de los logos*/
    </script>


    

    <script src="/bundles/jqueryval?v=hEGG8cMxk9p0ncdRUOJ-CnKN7NezhnPnWIvn6REucZo1"></script>
<script src="/bundles/Scripts/Inicio?v=WV9p_IYgd2MxSdWRKziXdPZOzsq9iDgv9BB4SfbMTos1"></script>


    <script>

        var shown = false;
        var currentModalidad = 0;
    var tiposEstudiosValues = [];
    var msjBusquedaSinCoincidenciasRNE = 'No existen coincidencias con los criterios de búsqueda utilizado, verifique su información y si el problema persiste puede escribirnos al correo electrónico: evaluaciondelacalidad@minerd.gob.do';

        var formarHTML = function () {

            var html = '';

            html += '<table id="tblRNE" class="table borderless" style="width:200px;"> ' +
                '	<tr> ' +
                '		<td colspan="2" style="text-align:left;"><label style="white-space:nowrap;"><u>Indique sus nombres y apellidos:</u></label></td>' +
                '	</tr>' +
                '	<tr> ' +
                '		<td style="width:13%; text-align:right;"><label style="white-space:nowrap;">Nombres: </label></td>' +
                '		<td style="padding:6px 0;"><input title="Primeros nombres" id="txtnombre" type="text" placeholder="Primeros nombres" style="color:black;" value="" /></td>' +
                '	</tr>' +
                '	<tr> ' +
                '		<td style="text-align:right;"><label style="white-space:nowrap;"> 1er Apellido: </label></td>' +
                '		<td style="padding:6px 0;"><input title="Primer apellido" id="txtapellido" type="text" style="color:black;" placeholder="1er Apellido" /></td>' +
                '	</tr>' +
                '	<tr> ' +
                '		<td style="text-align:right;"><label style="white-space:nowrap;">2do Apellido:</label></td>' +
                '		<td style="padding:6px 0;"><input id="txtapellido2" title="Segundo apellido" style="color:black;" type="text" placeholder="2do Apellido" /></td>' +
                '	</tr>' +
                '	<tr> ' +
                '		<td colspan="2" style="text-align:left;"><label style="white-space:nowrap;"><u>Fecha de nacimiento:</u></label></td>' +
                '	</tr>' +
                '	<tr> ' +
                '		<td style="text-align:right;"><label style="white-space:nowrap;">día:</label></td>' +
                '		<td style="padding:6px 0;"><input id="txtdia" title="Día de nacimiento" style="color:black; width:50px;" type="number" min="1" max="31" placeholder="día" /></td>' +
                '	</tr>' +
                '	<tr> ' +
                '		<td style="text-align:right;"><label style="white-space:nowrap;">mes:</label></td>' +
                '		<td style="padding:6px 0;"><input id="txtmes" title="Mes de nacimiento" style="color:black; width:50px;" type="number" min="1" max="12" placeholder="mes" /></td>' +
                '	</tr>' +
                '	<tr> ' +
                '		<td style="text-align:right;"><label style="white-space:nowrap;">año:</label></td>' +
                '		<td style="padding:6px 0;"><input id="txtanio" title="Año de nacimiento" style="color:black; width:50px;" type="number" placeholder="año" /></td>' +
                '	</tr>' +
                '	<tr> ' +
                '		<td colspan="2" style="text-align:center;"> <button onclick="buscarRNE();" style="background-color:#21374c;">Buscar RNE</button> </td>' +
                '	</tr>' +

                '	<tr id="test" style=" display:none;" > ' +
                '		<td style="text-align:right;"><label style="white-space:nowrap;">RNE:</label></td>' +
                '		<td style="padding:6px 0;"><p id="pRNE"></p></td>' +
                '	</tr>' +

                '</table>';

            return html;

        }

        var buscarRNE = function () {

            var validador = validarBuscadorRNE();

            if (validador.isValid) {
                var objeto = {
                    nombre: $('#txtnombre').val(),
                    apellido: $('#txtapellido').val(),
                    apellido2: $('#txtapellido2').val(),
                    dia: $('#txtdia').val(),
                    mes: $('#txtmes').val(),
                    anio: $('#txtanio').val()
                }

                ajaxCall(objeto, crearUrl('JsonCalls/buscarAyudaRNE'), 'POST', buscarRNE_callback);
            }
            else {
                toastr.error(validador.mensaje);
            }
        }

        var validarBuscadorRNE = function () {

            var validador = 1;

            var resultado = {
                isValid: true,
                mensaje: ''
            };

            validador *= $('#txtnombre').val().trim().length;
            validador *= $('#txtapellido').val().trim().length;
           // validador *= $('#txtapellido2').val().trim().length;
            validador *= $('#txtdia').val().trim().length;
            validador *= $('#txtmes').val().trim().length;
            validador *= $('#txtanio').val().trim().length;

            if (validador == 0) {
                resultado.isValid = false;
                resultado.mensaje = 'Por favor, complete todos los campos que se encuentren vacío';

                return resultado;
            }

            if ($('#txtnombre').val().trim().length < 2) {

                resultado.isValid = false;
                resultado.mensaje = 'El campo "Nombres" debe poseer al menos 2 caracteres.';

                return resultado;
            }

            if ($('#txtapellido').val().trim().length < 2) {

                resultado.isValid = false;
                resultado.mensaje = 'El campo "1er Apellido" debe poseer al menos 2 caracteres.';

                return resultado;
            }

            if ($('#txtdia').val().trim() < 1 || $('#txtdia').val().trim() > 31) {

                resultado.isValid = false;
                resultado.mensaje = 'El campo "Día de nacimiento" posee un formato inválido.';

                return resultado
            }

            if ($('#txtmes').val().trim() < 1 || $('#txtmes').val().trim() > 12) {

                resultado.isValid = false;
                resultado.mensaje = 'El campo "Mes de nacimiento" posee un formato inválido.';

                return resultado
            }

            if ($('#txtanio').val().trim() < 1) {

                resultado.isValid = false;
                resultado.mensaje = 'El campo "Año de nacimiento" posee un formato inválido.';

                return resultado
            }

            return resultado;
        }

        var buscarRNE_callback = function (data) {
            if (data.length == 1) {
                $('#txtRNE').val(data[0].RNE);
                limpiarBalloons();
            } else {
                $("#tblRNE").hide();
                $("#resultadosBusquedaRne").show();
                $("#resultados").html();
                for (x = 0; x < data.length; x++) {
                    $("#resultados").append(`<div style="padding: 15px;"><label><strong>Nombre: </strong>${data[x].RNE} - ${data[x].NombreCompleto}</label><label><strong>F. Nac: </strong>${data[x].FechaNacimiento}</label><a style="float: right;" href="#" class="seleccionar-rne" id="${data[x].RNE}">Seleccionar</a></div>`);
                }
                //Colocar rne en pantalla para que sea seleccionado
            }
        }

        var limpiarBalloons = function () {
            $('#aRNE').hideBalloon();
            shown = false;
        }

        $(function () {
            var showBallon = false;

            $("#drpTipoEstudios").change(function () {
                var val = $('#drpTipoEstudios').val();
                if (val != -1) {
                    var valueReplaced = val;
                    switch (valueReplaced) {
                        case "Conclusión de Estudios Medio":
                            currentModalidad = "41,42,43,44,45,46,47";
                            break;
                        case "Conclusión de Estudios Secundarios":
                        currentModalidad = "45,46,47";
                            break;
                        case "Conclusión de Estudios Básico":
                        currentModalidad = "1,31,32";
                            break;
                    }
                }
            });

            $(".nvl-opcion").click(function () {
                $("#panel-opciones").hide();
                $("#panel-datos").show();
                $('#drpTipoEstudios').val(-1);
                var id = $(this).prop("id");
                $('#txtRNE').val("");
                switch (id) {
                    case "nvlbasico":
                        $("#titleBasico").show();
                        $("#drpPeriodoEscolar").show();
                        $("#Convocatoria").show();
                        currentModalidad = "1,31,32";
                        break;
                    case "nvlmedio":
                        $("#titleMedio").show();
                        $("#drpPeriodoEscolar").show();
                        $("#Convocatoria").show();
                        currentModalidad = "41,42,43,44,45,46,47";
                        break;                   
                }
                initEvents();
            });

            $("#btn-volver").click(function () {
                $("#panel-opciones").show();
                $("#panel-datos").hide();
                $("#drpPeriodoEscolarProvisional").hide();
                $("#titleProvisional").hide();
                $("#TipoEstudio").hide();
                $("#titleMedio").hide();
                $("#drpPeriodoEscolar").hide();
                $("#Convocatoria").hide();
                $("#titleBasico").hide();
                $("#msjError").addClass("hidden");
                grecaptcha.reset();
            });

            $("#btnVolverResultado").click(function () {
                $("#resultadosBusquedaRne").hide();
                $("#tblRNE").show();
                showBallon = true;
            });

            $(".seleccionar-rne").click(function () {
                var rne = $(this).prop("id");
                $("#resultadosBusquedaRne").hide();
                showBallon = false;
                $("#tblRNE").hide();
                $('#txtRNE').val(rne);
            });

            $(document).on('click', ".seleccionar-rne", function() {
                var rne = $(this).prop("id");
                $("#resultadosBusquedaRne").hide();
                showBallon = false;
                $("#tblRNE").hide();
                $('#txtRNE').val(rne);
            });


            $(document).click(function () {
                if (!showBallon) {
                    limpiarBalloons();
                }
                showBallon = false;
            });

            $('#aRNE').on('click', function (e) {

                if (shown) {
                    $(this).hideBalloon()
                }
                else {
                    $('#aRNE').showBalloon({
                        tipSize: 6,
                        html: true,
                        contents: formarHTML(),
                        position: "top",
                        css: {
                            border: 'solid 1.2px #1d212b',
                            padding: '25px 10px 0 10px',
                            fontSize: '90%',
                            fontWeight: 'bold',
                            lineHeight: '3',
                            backgroundColor: '#151515',
                            color: '#fff'
                        }
                    });
                }

                shown = !shown

                $('#tblRNE').on('click', function (e) {
                    e.stopPropagation()
                });

                e.stopPropagation()
            });
        });
    </script>

</body>
</html>

