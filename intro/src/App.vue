<template>
    <div id='app' class='smallpcontainer'>
        <h1>Employees</h1>
        <employee-form />
        <employee-table :employees='employees' />
    </div>
</template>

<script>
import EmployeeTable from '@/components/EmployeeTable.vue'
import EmployeeForm from '@/components/EmployeeForm.vue'

export default {
    name: 'app',
    components: {
        EmployeeTable,
        EmployeeForm,
    },
    data() {
        return {
            employees: [
                {
                    id: 1, 
                    name: 'Tobie', 
                    email: 'Tobie@tobie.com'
                },
                {
                    id: 2,
                    name: 'Stacey',
                    email: 'Stacey@Stacey.com'
                },
                {
                    id: 3,
                    name: 'Mez',
                    email: 'Mez@Mez.com'
                },
            ]
        }
    }
}
</script>

<style>
button {
    background: #009435;
    border: 1px solid #009435;
}

.small-container {
    max-width: 680px;
}
</style>
