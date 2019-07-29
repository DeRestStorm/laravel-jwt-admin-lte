<template>
    <div class="wrapper">
        <header-component></header-component>


        <div class="content-wrapper">
            <router-view></router-view>
        </div>

        <!-- Control Sidebar -->
        <aside class="control-sidebar control-sidebar-dark">
            <!-- Control sidebar content goes here -->
            <div class="p-3">
                <h5>Title</h5>
                <p>Sidebar content</p>
            </div>
        </aside>
        <!-- /.control-sidebar -->
        <footer-component></footer-component>
    </div>
</template>
<script>
    import HeaderComponent from "./components/HeaderComponent";
    import FooterComponent from "./components/FooterComponent";

    export default {
        components: {
            HeaderComponent,
            FooterComponent
        }
    }
</script>