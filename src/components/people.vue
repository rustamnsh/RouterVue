<template>
  <div>
    <h1>My App</h1>
    <button v-on:click="getData">Data</button>
    
    <div v-for="Data in DataList" :key="Data.id" class="data">
        <br>
      <div class="stats">
     
        <table >
            <thead>
            <tr>
                <th>ID</th>
                <th>NAME</th>
                <th>VIP</th>
                <th>ATTENDING</th>
            </tr>
            </thead>
            <tbody>
            <td class="ID"><span>{{Data.id}}</span></td>
            <td class="NAME"><span>{{Data.name}}</span></td>
            <td class="VIP"><span>{{Data.vip}}</span></td>
            <td class="ATT"><span>{{Data.attending}}</span></td>
            </tbody>
        </table>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Data",
  data() {
    return {
      DataList: []
    };
  },
  methods: { 
    getData() {
      fetch("data.json")
        .then(response => response.json())
        .then(data => (this.DataList = data));
        
        
    }
  }
};

</script>