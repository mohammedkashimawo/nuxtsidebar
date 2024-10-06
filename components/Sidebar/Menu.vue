<script setup>
const items=  ref([
    {
        title:"overview",
        path:"/overview",
        icon:'ic:sharp-dashboard'


    },{

        title:'Transactions',
        path:'/transactions',
        icon:'subway:round-arrow-3'

        
        

    },{
        title:'Accounts',
        path:'/account',
        icon:'ic:sharp-account-balance'

    },{
        title:'Contacts',
        path:'/contact',
        icon:'tdesign:undertake-transaction'

    },{

        title:'Settings',
        path:"/settings",
        icon:'fluent:person-accounts-24-regular'

    }
])


</script>


<template>

<div>

    <header class="flex items-center gap-2 p-4  hover:scale-[101%] transition cursor-pointer">


<logo/>


<p class="font-bold"> ZAPexpress </p>

    </header><div class="px-4 grow">

<div class="grid gap-4">
<div v-for='( item,index) in items' :key='index' class="flex items-center gap-2 px-2 py-1
 transition rounded cursor-pointerhover:bg-neutral-100">

    <Icon size="20" :name="item.icon" color="black"/>
        
        <span>{{ item.title }}
    </span>


</div>

</div>




    </div>


</div>

</template>