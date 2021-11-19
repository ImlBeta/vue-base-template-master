<template>
<div>
  <p></p>
  <p></p>
  <h1>Formulario Validacion</h1>
    <label id="Nombre">Concesionario:</label>
    <input placeholder="Concesionario" type="text" v-model="name" class="redondeado" value="input con borde redondeado"  />
    <label id="Nombre"> Placa:</label>
    <input placeholder="Placa" type="text" v-model="placa" class="redondeado" value="input con borde redondeado"/>
    <label id="Nombre"> Ruta:</label>
    <input placeholder="Ruta" type="number" v-model="Ruta" class="redondeado" value="input con borde redondeado"/>
    <label id="Nombre"> Folio Solictud:</label>
    <input placeholder="Folio Solicitud" type="number" v-model="Folio" class="redondeado" value="input con borde redondeado"/>
    <label id="Nombre"> Identificacion:</label>
    <input placeholder="Identificacion" type="text" v-model="Identificacion" class="redondeado" value="input con borde redondeado"/>
    <br>
    <br>
    <label id="Nombre"> Titularidad:</label>
    <input placeholder="Titularidad" type="text" v-model="Titularidad" class="redondeado" value="input con borde redondeado"/>
    <label id="Nombre"> Fecha Emision:</label>
    <input placeholder="Fecha Emision" type="date" v-model="Fecha" class="redondeado" value="input con borde redondeado"/>
    <label id="Nombre"> Factura:</label>
    <input placeholder="Factura" type="text" v-model="Factura" class="redondeado" value="input con borde redondeado"/>
    <label id="Nombre"> NIV Factura:</label>
    <input placeholder="NIV Factura" type="text" v-model="NIVFac" class="redondeado" value="input con borde redondeado"/>
    <label id="Nombre"> Motor Factura:</label>
    <input placeholder="Motor Factura" type="text" v-model="MotFac" class="redondeado" value="input con borde redondeado"/>
                <!--<a-textarea placeholder="Autosize height based on content lines" />
    <a-input-search placeholder="input search loading deault" loading /> -->
    <br>
    <br>
    <a-button type="primary" html-type="submit" class="login-form-button">Validacion</a-button>
    <!--<button class="button button-close">X</button> -->
    </div>
</template>

<script>
export default {
  name: 'Input',
  data() {
    return {
      name: '',
      placa: '',
      Ruta: '',
      Folio: '',
      Identificacion: '',
      Titularidad: '',
      Fecha: '',
      Factura: '',
      NIVFac: '',
      MotFac: ''
    };
  }
};
</script>

<style>
.button {
    border: none;
    border-radius: 45px;
    background-color: red;
}

.buttonClose {
    text-align: right;
    background-color: red;
}

#Nombre
{
text-align: right;
color:rgb(17, 17, 17);
font-size: 15px;
font-family: Arial, Helvetica, sans-serif;
}
.redondeado {
   border-radius: 5px;
   background-color: #def;
 }
 .confondo {
   background-color: #def;
 }

</style>
