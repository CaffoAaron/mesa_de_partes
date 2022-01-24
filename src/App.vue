<template>
  <div>
    <header>
      <div class="navContainer backgroungRed" style="background-color: #85e772;">
        <div><a href="index.html"><img class="imgNavLeft" src="Images/logo-concytec_horizontal.png" alt="Gobierno del Perú"  style="width: 20%"/></a></div>
        <div><h1 class="navText">MESA DE PARTES DIGITAL</h1></div>
        <!--                <div><img class="imgNavRight" src="Images/cab_RRHH.gif" alt="PCM" width="240" /></div>-->
      </div>
    </header>
    <div class="main">
      <div class="container">
        <div class="flex-container">
          <div id="sidebar" class="sidebar">

            <div class="nav-side-menu">
              <i class="fa fa-bars fa-2x toggle-btn" data-toggle="collapse" data-target="#menu-content"></i>

              <div class="menu-list">

                <ul id="menu-content" class="menu-content collapse out">
                  <li>
                    <a href="Login/Indexa5bb.html" style="width: 100%; display:block;">
                      <i class="fa fa-home fa-lg"></i> Hola
                    </a>
                  </li>
                  <li data-toggle="collapse" data-target="#mant" class="collapsed">
                    <a href="#"><i class="fa fa-gift fa-lg"></i> Mantenimiento <span class="arrow"></span></a>
                  </li>
                  <ul class="sub-menu collapse" id="mant">
                    <li><a href="Login/Indexf660.html">Correo</a></li>
                    <li><a href="Login/Index8a21.html">Textos</a></li>
                    <li><a href="Login/Index1c24.html">Horarios</a></li>
                    <li><a href="Login/Index81bd.html">Peso documentos</a></li>
                  </ul>

                  <li data-toggle="collapse" data-target="#report" class="collapsed">
                    <a href="#" style="width: 100%; display:block;"><i class="fa fa-globe fa-lg"></i> Reportes <span class="arrow"></span></a>
                  </li>
                  <ul class="sub-menu collapse" id="report">
                    <li><a href="Login/Index81ab.html">Doc. pendientes</a></li>
                    <li><a href="Login/Index1140.html">Quiebres</a></li>
                  </ul>
                  <li>
                    <a href="Login/Indexa5bb.html" style="width: 100%; display:block;">
                      <i class="fa fa-sign-out-alt fa-lg"></i> Cerrar sesión
                    </a>
                  </li>
                </ul>
              </div>
            </div>

          </div>
          <div class="contentBody">




            <div class="panel panel-default">
              <div class="panel-heading text-center tituloHome">ENVÍO DE DOCUMENTOS</div>
              <div class="panel-body"><p>Estimados usuarios, para mayor facilidad, se ha puesto a su disposición este formulario, que le permitirá el envío de documentos a la Presidencia de Consejo de Ministros.</p><p>Esta modalidad de recepción estará activa en tanto dura la emergencia nacional declarada por D.S. N° 044-2020-PCM</p>
              </div>
            </div>

            <form action="https://mesapartesvirtual.pcm.gob.pe/" id="formDocumento" method="post">    <div class="panel panel-default">
              <div class="panel-heading subTituloHome">Datos del solicitante: </div>
              <div class="panel-body">

                <div class="col-md-10 col-md-offset-1">
                  <div class="row marginB-20">
                    <div class="form-group">
                      <div class="col-md-4">
                        <label for="IdTipoPersona" class="control-label">Tipo de persona</label>
                        <select class="form-control" id="IdTipoPersona" name="IdTipoPersona"><option value="03">CIUDADANO</option>
                          <option value="02">PERSONA JURIDICA</option>
                        </select>
                      </div>
                    </div>
                  </div>
                  <div id="divRuc" class="row marginB-20">

                    <div class="form-group">
                      <div class="col-md-4">
                        <label for="ruc" class="control-label">Nro de RUC</label>
                        <input type="text" class="form-control" id="ruc" placeholder="Nro de RUC" onkeypress="return isNumber(event)" />
                      </div>
                      <div class="col-md-8">
                        <label for="raz" class="control-label">Razón Social</label>
                        <input type="text" class="form-control" id="raz" placeholder="Razón Social" />
                      </div>

                    </div>
                    <label style="color:red;"> Recuerde que debe registrar datos de la persona de contacto</label>

                  </div>
                  <div class="row marginB-20">
                    <div class="form-group">
                      <div class="col-md-4">
                        <label for="dni" class="control-label">Nro DNI</label>
                        <input type="text" class="form-control" id="dni" placeholder="Nro DNI" onkeypress="return isNumber(event)" />
                      </div>
                    </div>
                  </div>
                  <div class="row marginB-20">
                    <div class="form-group">
                      <div class="col-md-4">
                        <label for="pat" class="control-label">Apellido paterno</label>
                        <input type="text" class="form-control" id="pat" placeholder="Apellido paterno" />
                      </div>
                      <div class="col-md-4">
                        <label for="mat" class="control-label">Apellido materno</label>
                        <input type="text" class="form-control" id="mat" placeholder="Apellido materno" />
                      </div>
                      <div class="col-md-4">
                        <label for="nom" class="control-label">Nombres</label>
                        <input type="text" class="form-control" id="nom" placeholder="Nombres" />
                      </div>
                    </div>
                  </div>
                  <div class="row marginB-20">
                    <div class="form-group">
                      <div class="col-md-4">
                        <label for="tel" class="control-label">Teléfono</label>
                        <input type="text" class="form-control" id="tel" placeholder="Teléfono" />
                      </div>
                    </div>
                  </div>
                  <div class="row marginB-20">
                    <div class="form-group">
                      <div class="col-md-4">
                        <label for="correo" class="control-label">Correo</label>
                        <input type="email" class="form-control" id="correo" placeholder="Correo" />
                      </div>
                    </div>
                  </div>
                  <div class="row marginB-20">
                    <div class="form-group">
                      <div class="col-md-12">
                        <label for="dir" class="control-label">Dirección</label>
                        <input type="text" class="form-control" id="dir" placeholder="Dirección" />
                      </div>
                    </div>
                  </div>

                </div>

              </div>
            </div>
              <div class="panel panel-default">
                <div class="panel-heading subTituloHome">Datos del documento: </div>
                <div class="panel-body">
                  <div class="col-md-10 col-md-offset-1">
                    <div class="row marginB-20">
                      <div class="form-group">
                        <div class="col-md-4">
                          <label for="IdTipoDocumento" class="control-label">Tipo de documento</label>
                          <select class="form-control" id="IdTipoDocumento" name="IdTipoDocumento"><option value="">[SELECCIONE]</option>
                            <option value="004">AYUDA MEMORIA</option>
                            <option value="233">CARTA</option>
                            <option value="005">DIRECTIVA</option>
                            <option value="015">EXPOSICI&#211;N DE MOTIVOS</option>
                            <option value="009">INFORME</option>
                            <option value="010">MEMORANDO</option>
                            <option value="234">MEMORANDO MULTIPLE</option>
                            <option value="013">NOTA DE ELEVACI&#211;N</option>
                            <option value="011">OFICIO</option>
                            <option value="250">OFICIO CIRCULAR</option>
                            <option value="012">OFICIO MULTIPLE</option>
                            <option value="238">OTROS</option>
                            <option value="232">PROVEIDO</option>
                            <option value="006">RESOLUCI&#211;N</option>
                            <option value="008">RESOLUCI&#211;N JEFATURAL</option>
                            <option value="016">RESOLUCI&#211;N VICEMINISTERIAL</option>
                            <option value="014">RESUMEN EJECUTIVO</option>
                            <option value="237">SOBRE CERRADO</option>
                            <option value="235">SOLICITUD</option>
                          </select>
                        </div>
                        <div class="col-md-4">
                          <label for="nrodoc" class="control-label">Nro de documento</label>
                          <input type="text" class="form-control" id="nrodoc" placeholder="Nro de documento" />
                        </div>
                      </div>
                    </div>
                    <div class="row marginB-20">
                      <div class="form-group">
                        <div class="col-md-4">
                          <label for="folios" class="control-label">Nro de folios</label>
                          <input type="text" class="form-control" id="folios" placeholder="Nro de folios" value="0" />
                        </div>
                      </div>
                    </div>
                    <div class="row marginB-20">
                      <div class="form-group">
                        <div class="col-md-12">
                          <label for="asu" class="control-label">Asunto</label>
                          <textarea class="form-control" id="asu" placeholder="Asunto" rows="4"></textarea>
                        </div>
                      </div>
                    </div>
                    <div class="row marginB-20">
                      <div class="form-group">
                        <div class="row" style="padding-left: 28px;">
                          <label class="control-label">Documento</label>
                        </div>
                        <div class="col-md-6">
                            <span class="control-fileupload">
                                <label for="fileDoc" class="truncateLongTexts">Escoge un archivo</label>
                                <input type="file" id="fileDoc" accept=".pdf">
                            </span>
                        </div>
                        <div class="col-md-2">
                          <button id="btnUpload" type="button" class="btn btn-default">
                            <i class="fa fa-file-upload"></i> CARGAR
                          </button>
                        </div>
                      </div>
                    </div>
                    <div class="row marginB-20">
                      <div class="form-group">
                        <div class="col-md-8">
                          <div class="panel panel-default">
                            <div class="panel-body">
                              <span id="mensajeDocumento">No ha seleccionado ningún archivo.</span>
                              <table id="tablaDocumento" class="table table-striped table-hover marginB-0" style="width: 100%; display: none;">
                                <thead>
                                <tr>
                                  <th>Nombre archivo</th>
                                  <th>Tipo</th>
                                  <th>Tamaño</th>
                                  <th>Acción</th>
                                </tr>
                                </thead>
                                <tbody></tbody>
                              </table>
                            </div>
                          </div>
                        </div>
                      </div>
                    </div>
                    <div class="row marginB-20">
                      <div class="form-group">
                        <div class="row" style="padding-left: 28px;">
                          <label class="control-label">Anexos [Opcional]</label>
                        </div>
                        <div class="col-md-6">
                            <span class="control-fileupload">
                                <label for="fileAnexo" class="truncateLongTexts">Escoge un archivo</label>
                                <input type="file" id="fileAnexo" accept=".pdf, .word, .jpg, .jpeg">
                            </span>
                        </div>
                        <div class="col-md-2">
                          <button id="btnUploadAnexo" type="button" class="btn btn-default">
                            <i class="fa fa-file-upload"></i> CARGAR
                          </button>
                        </div>
                      </div>
                    </div>
                    <div class="row marginB-20">
                      <div class="form-group">
                        <div class="col-md-8">
                          <div class="panel panel-default">
                            <div class="panel-body">
                              <span id="mensajeAnexo">No ha seleccionado ningún archivo.</span>
                              <table id="tablaAnexo" class="table table-striped table-hover marginB-0" style="width: 100%; display:none;">
                                <thead>
                                <tr>
                                  <th>Nombre archivo</th>
                                  <th>Tipo</th>
                                  <th>Tamaño</th>
                                  <th>Acción</th>
                                </tr>
                                </thead>
                                <tbody></tbody>
                              </table>
                            </div>
                          </div>
                        </div>
                      </div>
                    </div>

                    <div class="row marginB-20">
                      <div class="form-group text-center">
                        <button id="btnEnviar" type="submit" class="btn btn-danger">
                          ENVIAR
                        </button>
                      </div>
                    </div>

                    <div class="row marginB-20">
                      <div class="form-group">
                        <div class="col-md-2">
                          <label class="control-label">Nota</label>
                        </div>
                        <div class="col-md-10">
                          <ul><li>Para el documento principal el formato debe ser pdf</li><li>Para los anexos el formato puede ser pdf, word y jpg</li><li>Tamaño máximo de los archivos debe ser menor o igual a 50MB</li></ul>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>

              </div>
            </form>



          </div>
        </div>
      </div>
    </div>
    <footer class="backgroungRed text-center" style="background-color: #85e772;">
      <p>Oficina de Tecnologías de la Información</p>
    </footer>
  </div>
</template>

<script>


export default {
  name: 'App',
  components: {

  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
