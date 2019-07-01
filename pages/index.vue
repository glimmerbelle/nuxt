<template>
  <div>
    <div class="row">
      <div class="col-xl-8">
        <div class="kt-portlet kt-portlet--height-fluid kt-portlet--mobile ">
          <div class="kt-portlet__head kt-portlet__head--lg kt-portlet__head--noborder kt-portlet__head--break-sm">
            <div class="kt-portlet__head-label">
              <h3 class="kt-portlet__head-title">
                Exclusive Datatable Plugin
              </h3>
            </div>
            <div class="kt-portlet__head-toolbar">
              <div class="dropdown dropdown-inline">
                <button type="button" class="btn btn-clean btn-sm btn-icon btn-icon-md" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                  <i class="flaticon-more-1"></i>
                </button>
                <div class="dropdown-menu dropdown-menu-right dropdown-menu-md dropdown-menu-fit">

                  <!--begin::Nav-->
                  <ul class="kt-nav">
                    <li class="kt-nav__head">
                      Export Options
                      <i class="flaticon2-information" data-toggle="kt-tooltip" data-placement="right" title="Click to learn more..."></i>
                    </li>
                    <li class="kt-nav__separator"></li>
                    <li class="kt-nav__item">
                      <a href="#" class="kt-nav__link">
                        <i class="kt-nav__link-icon flaticon2-drop"></i>
                        <span class="kt-nav__link-text">Activity</span>
                      </a>
                    </li>
                    <li class="kt-nav__item">
                      <a href="#" class="kt-nav__link">
                        <i class="kt-nav__link-icon flaticon2-calendar-8"></i>
                        <span class="kt-nav__link-text">FAQ</span>
                      </a>
                    </li>
                    <li class="kt-nav__item">
                      <a href="#" class="kt-nav__link">
                        <i class="kt-nav__link-icon flaticon2-link"></i>
                        <span class="kt-nav__link-text">Settings</span>
                      </a>
                    </li>
                    <li class="kt-nav__item">
                      <a href="#" class="kt-nav__link">
                        <i class="kt-nav__link-icon flaticon2-new-email"></i>
                        <span class="kt-nav__link-text">Support</span>
                        <span class="kt-nav__link-badge">
                          <span class="kt-badge kt-badge--success">5</span>
                        </span>
                      </a>
                    </li>
                    <li class="kt-nav__separator"></li>
                    <li class="kt-nav__foot">
                      <a class="btn btn-label-danger btn-bold btn-sm" href="#">Upgrade plan</a>
                      <a class="btn btn-clean btn-bold btn-sm" href="#" data-toggle="kt-tooltip" data-placement="right" title="Click to learn more...">Learn more</a>
                    </li>
                  </ul>

                  <!--end::Nav-->
                </div>
              </div>
            </div>
          </div>
          <div class="kt-portlet__body kt-portlet__body--fit">

            <!--begin: Datatable -->
            <div class="kt-datatable" id="kt_datatable_latest_orders"></div>

            <!--end: Datatable -->
          </div>
        </div>
      </div>
      <div class="col-xl-4">

        <!--begin:: Widgets/Inbound Bandwidth-->
        <div class="kt-portlet kt-portlet--fit kt-portlet--head-noborder kt-portlet--height-fluid-half">
          <div class="kt-portlet__head kt-portlet__space-x">
            <div class="kt-portlet__head-label">
              <h3 class="kt-portlet__head-title">
                Inbound Bandwidth
              </h3>
            </div>
            <div class="kt-portlet__head-toolbar">
              <a href="#" class="btn btn-label-success btn-sm btn-bold dropdown-toggle" data-toggle="dropdown">
                Export
              </a>
              <div class="dropdown-menu dropdown-menu-fit dropdown-menu-right">
                <ul class="kt-nav">
                  <li class="kt-nav__item">
                    <a href="#" class="kt-nav__link">
                      <i class="kt-nav__link-icon flaticon2-line-chart"></i>
                      <span class="kt-nav__link-text">Reports</span>
                    </a>
                  </li>
                  <li class="kt-nav__item">
                    <a href="#" class="kt-nav__link">
                      <i class="kt-nav__link-icon flaticon2-send"></i>
                      <span class="kt-nav__link-text">Messages</span>
                    </a>
                  </li>
                  <li class="kt-nav__item">
                    <a href="#" class="kt-nav__link">
                      <i class="kt-nav__link-icon flaticon2-pie-chart-1"></i>
                      <span class="kt-nav__link-text">Charts</span>
                    </a>
                  </li>
                  <li class="kt-nav__item">
                    <a href="#" class="kt-nav__link">
                      <i class="kt-nav__link-icon flaticon2-avatar"></i>
                      <span class="kt-nav__link-text">Members</span>
                    </a>
                  </li>
                  <li class="kt-nav__item">
                    <a href="#" class="kt-nav__link">
                      <i class="kt-nav__link-icon flaticon2-settings"></i>
                      <span class="kt-nav__link-text">Settings</span>
                    </a>
                  </li>
                </ul>
              </div>
            </div>
          </div>
          <div class="kt-portlet__body kt-portlet__body--fluid">
            <div class="kt-widget20">
              <div class="kt-widget20__content kt-portlet__space-x">
                <span class="kt-widget20__number kt-font-brand">670+</span>
                <span class="kt-widget20__desc">Successful transactions</span>
              </div>
              <div class="kt-widget20__chart" style="height:130px;">
                <canvas id="kt_chart_bandwidth1"></canvas>
              </div>
            </div>
          </div>
        </div>

        <!--end:: Widgets/Inbound Bandwidth-->
        <div class="kt-space-20"></div>

        <!--begin:: Widgets/Outbound Bandwidth-->
        <div class="kt-portlet kt-portlet--fit kt-portlet--head-noborder kt-portlet--height-fluid-half">
          <div class="kt-portlet__head kt-portlet__space-x">
            <div class="kt-portlet__head-label">
              <h3 class="kt-portlet__head-title">
                Outbound Bandwidth
              </h3>
            </div>
            <div class="kt-portlet__head-toolbar">
              <a href="#" class="btn btn-label-warning btn-sm  btn-bold dropdown-toggle" data-toggle="dropdown">
                Download
              </a>
              <div class="dropdown-menu dropdown-menu-fit dropdown-menu-right">
                <ul class="kt-nav">
                  <li class="kt-nav__item">
                    <a href="#" class="kt-nav__link">
                      <i class="kt-nav__link-icon flaticon2-line-chart"></i>
                      <span class="kt-nav__link-text">Reports</span>
                    </a>
                  </li>
                  <li class="kt-nav__item">
                    <a href="#" class="kt-nav__link">
                      <i class="kt-nav__link-icon flaticon2-send"></i>
                      <span class="kt-nav__link-text">Messages</span>
                    </a>
                  </li>
                  <li class="kt-nav__item">
                    <a href="#" class="kt-nav__link">
                      <i class="kt-nav__link-icon flaticon2-pie-chart-1"></i>
                      <span class="kt-nav__link-text">Charts</span>
                    </a>
                  </li>
                  <li class="kt-nav__item">
                    <a href="#" class="kt-nav__link">
                      <i class="kt-nav__link-icon flaticon2-avatar"></i>
                      <span class="kt-nav__link-text">Members</span>
                    </a>
                  </li>
                  <li class="kt-nav__item">
                    <a href="#" class="kt-nav__link">
                      <i class="kt-nav__link-icon flaticon2-settings"></i>
                      <span class="kt-nav__link-text">Settings</span>
                    </a>
                  </li>
                </ul>
              </div>
            </div>
          </div>
          <div class="kt-portlet__body kt-portlet__body--fluid">
            <div class="kt-widget20">
              <div class="kt-widget20__content kt-portlet__space-x">
                <span class="kt-widget20__number kt-font-danger">1340+</span>
                <span class="kt-widget20__desc">Completed orders</span>
              </div>
              <div class="kt-widget20__chart" style="height:130px;">
                <canvas id="kt_chart_bandwidth2"></canvas>
              </div>
            </div>
          </div>
        </div>

        <!--end:: Widgets/Outbound Bandwidth-->
      </div>
    </div>
  </div>
</template>

<script>
export default {
  
}
</script>
