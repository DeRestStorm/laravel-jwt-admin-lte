<template>
    <header class="wrapper" style="height: auto;">
        <aside id="slider" class="main-sidebar">
            <section class="sidebar" style="height: auto;">
                <div class="user-panel">
                    <div class="pull-left image"><img
                            src="data:image/jpeg;base64,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"
                            alt="User Image" class="img-circle"></div>
                    <div class="pull-left info"><p>Alexander Pierce</p> <a href="#"><i class="fa fa-circle"
                                                                                       style="color: rgb(60, 118, 61);"></i>
                        Online</a></div>
                </div>
                <form action="#" method="get" class="sidebar-form">
                    <div class="input-group"><input type="text" name="q" placeholder="Search..." class="form-control">
                        <span class="input-group-btn"><button type="submit" name="search" id="search-btn"
                                                              class="btn btn-flat"><i class="fa fa-search"></i></button></span>
                    </div>
                </form>
                <ul class="sidebar-menu">
                    <li class="header">
                        MAIN NAVIGATION
                        <!----> <!----></li>
                    <li class="treeview">

                        <a href="#"><i class="fa fa-dashboard"></i> <span>Dashboard</span> <span
                                class="pull-right-container"><i class="fa fa-angle-left pull-right"></i></span></a>
                        <ul class="treeview-menu">
                            <li class="active"><a href="/"><i class="fa fa-circle-o"> 헬로화면</i></a></li>
                            <li class=""><a href="/sample"><i class="fa fa-circle-o"> 샘플화면</i></a></li>
                            <li class=""><a href="/dashboard/v1"><i class="fa fa-circle-o"> Dashboard v1</i></a></li>
                            <li class=""><a href="/dashboard/v2"><i class="fa fa-circle-o"> Dashboard v2</i></a></li>
                            <li class=""><a href="/examples/infobox"><i class="fa fa-circle-o"> InfoBox</i></a></li>
                            <li class=""><a href="/examples/chart"><i class="fa fa-circle-o"> Chart.js</i></a></li>
                            <li class=""><a href="/examples/alert"><i class="fa fa-circle-o"> Alert</i></a></li>
                            <li class=""><a href="/examples/modal"><i class="fa fa-circle-o"> Modal</i></a></li>
                            <li class=""><a href="/examples/api-example"><i class="fa fa-circle-o"> APIExample</i></a>
                            </li>
                        </ul>
                    </li>
                    <li class="treeview">

                        <a href="#"><i class="fa fa-files-o"></i> <span>Layout Options</span> <span
                                class="pull-right-container"><small class="label pull-right label-primary">4</small></span></a>
                        <ul class="treeview-menu">
                            <li><a><i class="fa fa-circle-o"> Top Navigation</i></a></li>
                            <li><a><i class="fa fa-circle-o"> Boxed</i></a></li>
                            <li><a><i class="fa fa-circle-o"> Fixed</i></a></li>
                            <li><a><i class="fa fa-circle-o"> Collapsed Sidebar</i></a></li>
                        </ul>
                    </li>
                    <li class=""><a href="/examples/widgets"><i class="fa fa-th"></i> <span>Widgets</span> <span
                            class="pull-right-container"><small
                            class="label pull-right bg-green">new</small></span></a></li>
                    <li class="treeview">

                        <a href="#"><i class="fa fa-laptop"></i> <span>UI Elements</span> <span
                                class="pull-right-container"><i class="fa fa-angle-left pull-right"></i></span></a>
                        <ul class="treeview-menu">
                            <li class=""><a href="/ui-elements/general"><i class="fa fa-circle-o"> General</i></a></li>
                            <li class=""><a href="/ui-elements/icons"><i class="fa fa-circle-o"> Icons</i></a></li>
                            <li class=""><a href="/ui-elements/buttons"><i class="fa fa-circle-o"> Buttons</i></a></li>
                            <li class=""><a href="/ui-elements/sliders"><i class="fa fa-circle-o"> Sliders</i></a></li>
                            <li class=""><a href="/ui-elements/timeline"><i class="fa fa-circle-o"> Timeline</i></a>
                            </li>
                            <li class=""><a href="/ui-elements/modals"><i class="fa fa-circle-o"> Modals</i></a></li>
                        </ul>
                    </li>
                    <li class="treeview">

                        <a href="#"><i class="fa fa-edit"></i> <span>Forms</span> <span class="pull-right-container"><i
                                class="fa fa-angle-left pull-right"></i></span></a>
                        <ul class="treeview-menu">
                            <li class=""><a href="/forms/general-elements"><i class="fa fa-circle-o"> General
                                Elements</i></a></li>
                            <li class=""><a href="/forms/advanced-elements"><i class="fa fa-circle-o"> Advanced
                                Elements</i></a></li>
                            <li><a><i class="fa fa-circle-o"> Editors</i></a></li>
                        </ul>
                    </li>
                </ul>
            </section>
        </aside>
        <div id="content-wrap" class="content-wrapper" style="min-height: 926px;">
            <section class="content-header">
                <h1>
                    Dashboard
                    <small>Version 2.0</small>
                </h1>
                <ol class="breadcrumb">
                    <li><a href="#"><i class="fa fa-dashboard"></i> Home</a></li>
                    <li class="active">Dashboard</li>
                </ol>
            </section>
            <section class="content"><!----></section>
        </div>
        <div id="bsModal" tabindex="-1" role="dialog" aria-labelledby="bsModalLabel" data-toggle="modal"
             data-backdrop="static" data-keyboard="false" class="modal fade">
            <div role="document" class="modal-dialog">
                <div class="modal-content">
                    <div class="modal-header">
                        <button type="button" data-dismiss="modal" aria-label="Close" class="close"><span
                                aria-hidden="true">×</span></button>
                        <h4 id="bsModalLabel" class="modal-title"></h4></div>
                    <div class="modal-body">

                    </div>
                    <div class="modal-footer">
                        <button type="button" class="btn btn-default"></button>
                        <button type="button" class="btn btn-primary"></button>
                    </div>
                </div>
            </div>
        </div>
    </header>
</template>