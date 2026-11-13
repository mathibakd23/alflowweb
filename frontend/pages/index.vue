<script setup lang="ts">
const debtors=["Novo Pharma","Novo Kalundborg","Arla Foods"]
const products=[{name:'Dockweiler Tube 25x1.6',price:275},{name:'EPDM Gasket',price:42},{name:'Tri Clamp',price:95}]
</script>
<template><div><h1>Dashboard</h1><label>Aktiv debitor <select><option v-for="d in debtors">{{d}}</option></select></label><h2>Produktoversigt</h2><div v-for="p in products" :key="p.name" style="border:1px solid #ddd;padding:8px;margin:8px 0">{{p.name}} - {{p.price}} kr.</div></div></template>