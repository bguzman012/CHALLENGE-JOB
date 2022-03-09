<template>
  <div class="container" style="margin-top: 15px">
    <div>


    </div>

    <div style="text-align: center">
      <b-form
        inline
        style="
          margin-top: 25px;
          text-align: center;
          padding: 40px 25px;
          border-radius: 8px;
          background-color: #270570;
          box-shadow: 0 4px 8px rgba(68, 68, 68, 0.2);
          box-sizing: border-box;
        "
      >
        <div
          class="form-group col-xs-6"
          style="background-color: #fff; margin-right: 15px; padding: 10px; border-radius: 10px"
        >
          <vue-bootstrap-typeahead 
          placeholder="Inicio"
  :data="['Azuay', 'Pichincha', 'Napo', 'Bogota', 'JFK', 'Berlin', 'Pastaza', 'Asuncion']"
/>
 <vue-bootstrap-typeahead 
          placeholder="Destino"
  :data="['Azuay', 'Pichincha', 'Napo', 'Bogota', 'JFK', 'Berlin', 'Pastaza', 'Asuncion']"
/>
        </div>

        <div
          class="form-group col-xs-6"
          style="background-color: #fff; padding: 10px; border-radius: 10px"
        >
          <b-form-datepicker
            :state="true"
            id="datepicker-valid"
            placeholder="ida"
            today-button
            :date-format-options="{
              year: 'numeric',
              month: 'short',
              day: '2-digit',
              weekday: 'short',
            }"
            locale="es"
            style="margin-right: 5px; width: 225px"
          ></b-form-datepicker>

          <b-form-datepicker
            id="datepicker-invalid"
            :state="false"
            locale="es"
            :date-format-options="{
              year: 'numeric',
              month: 'short',
              day: '2-digit',
              weekday: 'short',
            }"
            placeholder="vuelta"
            style="width: 225px"
          ></b-form-datepicker>
        </div>

        <b-button
          variant="primary"
          style="
            height: 48px;
            padding: 0 20px;
            margin-left: 30px;
            font-size: 16px;
            line-height: 48px;
          "
          >Search</b-button
        >
      </b-form>
      
    </div>
  </div>
</template>

