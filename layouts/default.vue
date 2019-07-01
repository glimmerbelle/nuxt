<template>
  <div>
    
    <HeaderMobile/>
    <div class="kt-grid kt-grid--hor kt-grid--root">
			<div class="kt-grid__item kt-grid__item--fluid kt-grid kt-grid--ver kt-page">
        <Aside/>
        <div class="kt-grid__item kt-grid__item--fluid kt-grid kt-grid--hor kt-wrapper" id="kt_wrapper">
          <Header/>
          <div class="kt-grid__item kt-grid__item--fluid kt-grid kt-grid--hor">
            <SubHeader/>
            <div class="kt-content  kt-grid__item kt-grid__item--fluid" id="kt_content">
              <nuxt />
            </div>
          </div>
          <Footer/>
        </div>
      </div>
    </div>
    <QuickPanel/>
    <ScrollTop />
    

      
      
        
      </div>
    </div>
  </div>
</template>
<script>
import Header from '~/components/Navigation/Header'
import HeaderMobile from '~/components/Navigation/HeaderMobile'
import QuickPanel from '~/components/Navigation/QuickPanel'
import ScrollTop from '~/components/Navigation/ScrollTop'
import Aside from '~/components/Navigation/Aside'
import SubHeader from '~/components/Navigation/SubHeader'
import Footer from '~/components/Partials/Footer'

export default{
  mounted(){
    WebFont.load({
				google: {
					"families": ["Poppins:300,400,500,600,700", "Roboto:300,400,500,600,700"]
				},
				active: function() {
					sessionStorage.fonts = true;
				}
      });
      var KTAppOptions = {
				"colors": {
					"state": {
						"brand": "#22b9ff",
						"light": "#ffffff",
						"dark": "#282a3c",
						"primary": "#5867dd",
						"success": "#34bfa3",
						"info": "#36a3f7",
						"warning": "#ffb822",
						"danger": "#fd3995"
					},
					"base": {
						"label": ["#c5cbe3", "#a1a8c3", "#3d4465", "#3e4466"],
						"shape": ["#f0f3ff", "#d9dffa", "#afb4d4", "#646c9a"]
					}
				}
			};
  },
  head () {
    return {
      title: this.title,
      meta: [
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        { charset: 'utf-8'},
        { hid: 'description', name: 'description', content: 'Latest updates and statistic charts' },
        { name: 'viewport', content: 'width=device-width, initial-scale=1, shrink-to-fit=no'}
      ],
      bodyAttrs: {
        class: 'kt-quick-panel--right kt-demo-panel--right kt-offcanvas-panel--right kt-header--fixed kt-header-mobile--fixed kt-subheader--enabled kt-subheader--transparent kt-aside--enabled kt-aside--fixed kt-aside--minimize kt-page--loading',
      },
      
    }
  },
  components:{
    Header,
    QuickPanel,
    HeaderMobile,
    ScrollTop,
    Aside,
    Footer,
    SubHeader
  },
  data(){
    return{
      title: 'Cityield'
    }
  }
}
</script>
