<template>
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <paper-table :title="table1.title" :sub-title="table1.subTitle" :data="table1.data" :columns="table1.columns">

          </paper-table>
        </div>
      </div>

    </div>
</template>
<script>
  import PaperTable from 'components/UIComponents/PaperTable.vue'
  const tableColumns = ['Id', 'Name', 'Price', 'CreatedAt', 'UpdatedAt', 'SellerName']
  const tableData = [{
    id: 1,
    name: 'T-shirt',
    price: '5000',
    createdat: '15/2/2018',
    updatedat: '16/2/2018',
    sellername: 'Sama Walid'
  },
  {
    id: 2,
    name: 'Mobile',
    price: '3000',
    createdat: '15/2/2018',
    updatedat: '16/2/2018',
    sellername: 'Ziad Hossam'
  },
  {
    id: 3,
    name: 'glasses',
    price: '2000',
    createdat: '15/2/2018',
    updatedat: '16/2/2018',
    sellername: 'Mohamed Saeed'
  },
  {
    id: 4,
    name: 'cups',
    price: '3000',
    createdat: '15/2/2018',
    updatedat: '16/2/2018',
    sellername: 'Nourhan Ali'
  },
  {
    id: 5,
    name: 'Windows',
    price: '1000',
    createdat: '15/2/2018',
    updatedat: '16/2/2018',
    sellername: 'Amr Elarabi'
  }]

  export default {
    components: {
      PaperTable
    },
    data () {
      return {
        table1: {
          title: 'Store Component 3',
          subTitle: 'Ebay',
          columns: [...tableColumns],
          data: [...tableData]
        },
        table2: {
          title: 'Table on Plain Background',
          subTitle: 'Here is a subtitle for this table',
          columns: [...tableColumns],
          data: [...tableData]
        }
      }
    }
  }

</script>
<style>

</style>
