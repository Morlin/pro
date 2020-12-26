<template>
    <div>
        <div class="position-relative">
            <!-- shape Hero -->
            <section class="section-shaped my-0">
                <div class="shape shape-style-1 shape-default shape-skew">
                    <span></span>
                </div>
                <div class="container shape-container d-flex">
                    <div class="col px-0">
                        <div class="row">
                            <div class="col-lg-12">
                                <h1 class="display-3  text-white">
                                    {{$t('helloFriends')}}<br/>
                                    <span>{{$t('needUpgrade')}}</span>
                                </h1>
                                 <card gradient="warning" no-body shadow-size="lg" class="border-0">
                                    <div class="p-5">
                                        <div class="row align-items-center">
                                            <div class="col-lg-8">
                                                <h3 class="text-white">{{$t('btn.join')}}</h3>
                                            </div>
                                            <div class="col-lg-3 ml-lg-auto">
                                                <base-button tag="a" href="#" type="white" block size="lg" @click="modals.register = true">
                                                    {{$t('btn.reigsterFor')}}&nbsp;$150
                                                </base-button>
                                                <modal :show.sync="modals.register" gradient="danger" modal-classes="modal-danger modal-dialog-centered">
                                                    <h6 slot="header" class="modal-title" id="modal-title-notification">Your attention is required</h6>
                                                    <div class="py-3 text-center">
                                                        <i class="ni ni-bell-55 ni-3x"></i>
                                                        <h4 class="heading mt-4">You should read this!</h4>
                                                        <p>A small river named Duden flows by their place and supplies it with the necessary regelialia.</p>
                                                    </div>
                                                    <template slot="footer">
                                                        <base-button type="white">Ok, Got it</base-button>
                                                        <base-button type="link" text-color="white" class="ml-auto" @click="modals.register = false">
                                                            Close
                                                        </base-button>
                                                    </template>
                                                </modal>
                                            </div>
                                        </div>
                                    </div>
                                </card>
                                <p class="lead text-white">{{$t('longSpeech.1')}}<br/>{{$t('longSpeech.2')}}<br/>{{$t('longSpeech.3')}}<br/>{{$t('longSpeech.4')}}</p>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
        </div>
        <section class="section section-lg  pt-lg-0 mt--200">
            <div class="container">
                <div class="row row-grid align-items-center">
                    <div class="col-md-6 order-md-2">
                        <div class="card bg-default shadow border-0">
                            <img v-lazy="'img/theme/11.jpg'" class="card-img-top">
                            <blockquote class="card-blockquote">
                                <svg preserveAspectRatio="none" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 583 95"
                                     class="svg-bg">
                                    <polygon points="0,52 583,95 0,95" class="fill-default"></polygon>
                                    <polygon points="0,42 583,95 683,0 0,95" opacity=".2" class="fill-default"></polygon>
                                </svg>
                                
                                <p class="lead text-italic text-white">{{$t('offer')}}</p>
                            </blockquote>
                        </div>
                    </div>
                    <div class="col-md-6 order-md-1">
                        <div class="pr-md-5">
                            <h3>{{$t('whatYouGet')}}</h3>
                            <p>{{$t('offer')}}</p>
                            <ul class="list-unstyled mt-5">
                                <li class="py-2">
                                    <div class="d-flex align-items-center">
                                        <badge type="success" circle class="mr-3" icon="ni ni-settings-gear-65"></badge>
                                        <h6 class="mb-0">{{$t('whatYouGet1')}}</h6>
                                    </div>
                                </li>
                                <li class="py-2">
                                    <div class="d-flex align-items-center">
                                        <badge type="success" circle class="mr-3" icon="ni ni-html5"></badge>
                                        <h6 class="mb-0">{{$t('whatYouGet2')}}</h6>
                                    </div>
                                </li>
                                <li class="py-2">
                                    <div class="d-flex align-items-center">
                                        <badge type="success" circle class="mr-3" icon="ni ni-satisfied"></badge>
                                        <h6 class="mb-0">{{$t('whatYouGet3')}}</h6>
                                    </div>
                                </li>
                                <li class="py-2">
                                    <div class="d-flex align-items-center">
                                        <badge type="success" circle class="mr-3" icon="ni ni-html5"></badge>
                                        <h6 class="mb-0">{{$t('whatYouGet4')}}</h6>
                                    </div>
                                </li>
                                <li class="py-2">
                                    <div class="d-flex align-items-center">
                                        <badge type="success" circle class="mr-3" icon="ni ni-satisfied"></badge>
                                        <h6 class="mb-0">{{$t('whatYouGet5')}}</h6>
                                    </div>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        <section class="section section-lg pt-0">
            <div class="container">
                <card gradient="warning" no-body shadow-size="lg" class="border-0">
                    <div class="p-5">
                        <div class="row align-items-center">
                            <div class="col-lg-8">
                                <p class="lead text-white mt-3">{{$t('myMotivation')}}</p>
                            </div>
                            <div class="col-lg-3 ml-lg-auto">
                                <base-button tag="a" href="#" type="white" block size="lg" @click="modals.register = true">
                                    {{$t('btn.reigsterFor')}}&nbsp;$150
                                </base-button>
                            </div>
                        </div>
                    </div>
                </card>
            </div>
        </section>
        <section class="section section-lg pt-lg-0">
            <div class="container">
                <div class="row justify-content-center">
                    <div class="col-lg-12">
                        <div class="row row-grid">
                            <div class="col-lg-4">
                                <card class="border-0" hover shadow body-classes="py-5">
                                    <h6 class="text-primary text-uppercase">
                                        {{$t('programIncludes1')}}</h6>
                                    <div>
                                        <badge type="primary" rounded>design</badge>
                                        <badge type="primary" rounded>system</badge>
                                        <badge type="primary" rounded>creative</badge>
                                    </div>
                                </card>
                            </div>
                            <div class="col-lg-4">
                                <card class="border-0" hover shadow body-classes="py-5">
                                    <h6 class="text-success text-uppercase">
                                        {{$t('programIncludes2')}}</h6>
                                    <div>
                                        <badge type="success" rounded>business</badge>
                                        <badge type="success" rounded>vision</badge>
                                        <badge type="success" rounded>success</badge>
                                    </div>
                                </card>
                            </div>
                            <div class="col-lg-4">
                                <card class="border-0" hover shadow body-classes="py-5">
                                    <h6 class="text-warning text-uppercase">
                                         {{$t('programIncludes3')}}</h6>
                                    <div>
                                        <badge type="warning" rounded>marketing</badge>
                                        <badge type="warning" rounded>product</badge>
                                        <badge type="warning" rounded>launch</badge>
                                    </div>
                                </card>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        
        <section class="section section-shaped my-0 overflow-hidden">
            <div class="shape shape-style-3 bg-gradient-default shape-skew">
                <span></span>
            </div>
            <div class="container">
                <div class="row text-center justify-content-center">
                     <div class="col-lg-8">
                        <card gradient="secondary" shadow body-classes="p-lg-5">
                            <h4 class="mb-1">Want to work with us?</h4>
                            <p class="mt-0">Your project is very important to us.</p>
                            <base-input class="mt-5"
                                        alternative
                                        placeholder="Your name"
                                        addon-left-icon="ni ni-user-run">
                            </base-input>
                            <base-input alternative
                                        placeholder="Email address"
                                        addon-left-icon="ni ni-email-83">
                            </base-input>
                            <base-input class="mb-4">
                                    <textarea class="form-control form-control-alternative" name="name" rows="4"
                                              cols="80" placeholder="Type a message..."></textarea>
                            </base-input>
                            <base-button type="default" round block size="lg">
                                Send Message
                            </base-button>
                        </card>
                    </div>
                </div>
            </div>
        </section>
    </div>
    
</template>

<script>
import Modal from "@/components/Modal.vue";
export default {
  components: {
    Modal
  },
  name: "home",
  data() {
    return {
      modals: {
        register: false
      }
    };
  }
};
</script>