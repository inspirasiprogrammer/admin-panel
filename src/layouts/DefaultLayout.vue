<template>
  <!-- Sidebar -->
  <sidebar />
  <!-- Content Container-->
  <div class="min-h-screen">
    <navbar />
    <!-- Content. In actually use, this must be a router-view-->
    <div class="ml-64 pt-14 px-5">
      <div class="container mx-auto my-5">
        <div class="grid gap-5 sm:grid-cols-2 lg:grid-cols-4">
          <div class="bg-green-50 rounded-xl p-5">
            <credit-card-icon-o class="w-10 h-10 text-green-500" />
            <p class="mt-8 text-green-500 text-sm">Transfer via card number</p>
          </div>
          <div class="bg-purple-50 rounded-xl p-5">
            <chart-pie-icon-o class="w-10 h-10 text-purple-500" />
            <p class="mt-8 text-purple-500 text-sm">Transfer to another bank</p>
          </div>
          <div class="bg-yellow-50 rounded-xl p-5">
            <user-group-icon-o class="w-10 h-10 text-yellow-500" />
            <p class="mt-8 text-yellow-500 text-sm">Transfer to the same bank</p>
          </div>
          <div class="bg-blue-50 rounded-xl p-5">
            <library-icon-o class="w-10 h-10 text-blue-500" />
            <p class="mt-8 text-blue-500 text-sm">Request cash withdrawals</p>
          </div>
        </div>
      </div>      
    </div>
  </div>
</template>

<script>
import Sidebar from '@/components/layouts/Sidebar.vue';
import Navbar from '@/components/layouts/Navbar.vue';
export default {
  components: {
    Sidebar,
    Navbar
  }
}
</script>