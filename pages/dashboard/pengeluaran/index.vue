<template>
    <div class="dashboard">
        <Header/>
        <section class="columns">
            <aside class="column is-3 side-menu-container is-hidden-mobile">
                <Sidebar/>
                <!-- <Sidebar @onLogout="logout"/> -->
            </aside>
            <div class="column dashboard-column">
                <section class="dashboard-content">
                    <Orders/>
                </section>
            </div>
        </section>
    </div>
</template>

<script>
    import Header from '../../../components/pages/dashboard/Header'
    import Sidebar from '@/components/pages/dashboard/Sidebar'
    import Orders from "@/components/pages/dashboard/Outcomes"
    export default {
        components: { Header, Sidebar, Orders},
    }
</script>

<style unscoped>
  @import url('https://fonts.googleapis.com/css?family=Quicksand:300,400,500,700');
  body {
	font-family: 'Quicksand', sans-serif;
    color: rgb(90, 80, 80);
    letter-spacing: 0.5px;
    font-weight: 400;
  }
  .dashboard {
    font-size: 16px;
    line-height: 1.5;
    height: 100%;
  }
  aside.column.side-menu-container {
    padding: 7rem 1rem 2rem 2rem;
    background-color: #7e72b1;
    opacity: 20%;
    color: white;
    min-height: 105vh;
  }
  .is-hidden-tablet {
   background-color: #7e72b1;
    opacity: 20%;
    color: white;
  }
  .dashboard-column {
    background-color: #FFF;
    padding: 4rem 1rem 2rem 1rem;
  }
  .dashboard-content {
    padding: 15px 15px;
    &__metrics {
      border: 1px solid #999;
      padding:1rem 0rem;
    }
    &__metrics-item {
      p {
          color: #9f00bf; 
      }
    }
  }
  @media (max-width: 837px) {
	  aside.column.side-menu-container {
      min-width: 215px;
      min-height: auto;
    }
  }  
  @media (max-width: 768px) {
	  aside.column.side-menu-container {
      min-height: auto;
    }
  }
</style>