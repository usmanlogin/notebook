<script setup>
import { reactive } from 'vue'

let state = reactive({
  show_menu: false,
  active_tab: 'three'
})
</script>

<template>
  <div class="header_bg">

    <!-- Navbar start -->
    <div class="border-bottom header-border">
      <div class="container">
        <nav class="navbar navbar-expand-lg py-3">
          <div class="container-fluid">
            <a class="navbar-brand" href="#">
              <img src="@/assets/images/logo.svg" />
            </a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
              @click="state.show_menu = !state.show_menu" data-bs-target="#navbarSupportedContent"
              aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
              <span class="navbar-toggler-icon"></span>
            </button>
            <div class=" navbar-collapse" :class="state.show_menu ? '' : 'collapse'" id="navbarSupportedContent">
              <ul class="navbar-nav me-auto mb-2 mb-lg-0 px-0 px-lg-5 mt-1">
                <li class="nav-item px-0 px-lg-3">
                  <a class="nav-link active" aria-current="page" href="#">Home</a>
                </li>

                <li class="nav-item dropdown px-0 px-lg-3">
                  <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-bs-toggle="dropdown"
                    aria-expanded="false">
                    Community
                  </a>
                  <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
                    <li><a class="dropdown-item" href="#">Action</a></li>
                    <li><a class="dropdown-item" href="#">Another action</a></li>
                    <li>
                      <hr class="dropdown-divider" />
                    </li>
                    <li><a class="dropdown-item" href="#">Something else here</a></li>
                  </ul>
                </li>
                <li class="nav-item px-0 px-lg-3">
                  <a class="nav-link" href="#">Blogs</a>
                </li>
                <li class="nav-item px-0 px-lg-3">
                  <a class="nav-link" href="#">Events</a>
                </li>
              </ul>
              <form class="d-flex  flex-lg-row flex-column">
                <div class="mx-0 mx-lg-5 relative border-bottom">
                  <img src="@/assets/images/search.svg" class="search-icon" />
                  <input class="form-control search-bar shadow-none py-2 pl-5" type="search" placeholder="Search here..."
                    aria-label="Search here" />
                </div>
                <button class="btn btn-primary text-white btn-login mt-3 mt-lg-0" type="submit">Log in</button>
              </form>
            </div>
          </div>
        </nav>
      </div>
    </div>
    <!-- NavbarEnd -->

    <!-- Banner -->
    <div class="container">
      <div class="row align-items-center pb-md-5 pb-sm-3 pb-xs-2">
        <div class="col comunity_col p-3 py-5">
          <button class="btn btn-primary btn_light text-primary">Netbook Community</button>
          <h1 class="fw-bold mt-4">Your Solutions For Community!</h1>
          <p class="text_gray font_normal mt-4">
            More than 2 billion people in over countries use socibook to stay in touch with friends
            & family.
          </p>
          <div class="d-flex mt-5">
            <button class="btn btn-primary text-white">About More</button>
            <button class="btn btn-outline-primary fw_normal mx-3">Invite Friend</button>
          </div>
        </div>
        <div class="col p-3 d-none d-md-block">
          <img src="@/assets/images/group.svg" class="img-fluid" />
        </div>
      </div>
    </div>
    <!-- banner end -->
  </div>
  <!-- header-ending -->

  <!-- Social Network -->
  <div class="container">
    <div class="row align-items-center py-5">
      <div class="col-sm-12 col-md-6 py-4">
        <div class="social_box">
          <a href="#" class="text-decoration-none fw_normal">Whats Netboks?</a>
          <h2 class="fw-bold mt-2">Why Join to Netbook Social Network?</h2>
          <p class="mt-3 text_gray">
            Recent surveys have indicated that small businesses recognise the need they have to
            connect with consumer.
          </p>
          <ul class="mt-4 list-unstyled">
            <li class="flex mt-2">
              <img src="@/assets/images/radio.svg" /><span class="px-2 fw_normal">Groups</span>
            </li>
            <li class="flex mt-2">
              <img src="@/assets/images/radio.svg" /><span class="px-2 fw_normal">Messages</span>
            </li>
            <li class="flex mt-2">
              <img src="@/assets/images/radio.svg" class="" /><span class="px-2 fw_normal">Share</span>
            </li>
          </ul>
        </div>
      </div>
      <div class="col-sm-12 col-md-6 py-4">
        <div class="row">
          <div class="col justify-content-end d-flex">
            <img src="@/assets/images/about_one.svg" class="img-fluid" />
          </div>
          <div class="col">
            <div class="d-flex justify-content-end">
              <img src="@/assets/images/about_two.svg" class="img-fluid float-end w_full" />
            </div>
            <div class="mt-4 d-flex justify-content-end">
              <img src="@/assets/images/about_three.svg" class="img-fluid float-end w_full" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Digital life -->
  <div class="container">
    <div class="row align-items-center py-4">
      <div class="col-md-12 col-lg-4 mt-5">
        <div class="p-5 border rounded-4 life_box">
          <div class="d-flex align-items-center">
            <img src="@/assets/images/star.svg" class="" />
            <h4 class="font_large my-auto px-2">4.8 Rating</h4>
          </div>

          <div class="d-flex space-x-2 mt-3">
            <div class="ms-n3">
              <img src="@/assets/images/people.svg" class="pt-2" />
            </div>

            <h4 class="self-center font_normal my-auto">
              <span class="text-primary fw-medium">+836</span> Members
            </h4>
          </div>

          <p class="text_light mt-4">
            More than 2 billion we people over countries use socibooks we to stay in touch with
            friends.
          </p>

          <div class="mt-5">
            <a href="#" class="text-primary text-decoration-none">
              <span class="text-decoration-none fw_normal">Join Our Community</span>
              <img src="@/assets/images/arrow-right-blue.svg" class="ms-2" />
            </a>
          </div>
        </div>
      </div>
      <div class="col-md-12 col-lg-4 col-md-4 mt-5">
        <div class="p-5 border rounded-4 life_box">
          <div class="d-flex align-items-center">
            <img src="@/assets/images/trophy.svg" class="" />
            <h4 class="font_large my-auto px-2">Awwwards</h4>
          </div>

          <div class="d-flex space-x-2 mt-3">
            <div class="ms-n3">
              <img src="@/assets/images/github.svg" class="pt-2" />
            </div>

            <h4 class="self-center font_normal my-auto">
              Best of <span class="text-primary fw-medium">2021</span> on Github
            </h4>
          </div>

          <p class="text_light mt-4">
            More than 2 billion we people over countries use socibooks we to stay in touch with
            friends.
          </p>

          <div class="mt-5">
            <a href="#" class="text-decoration-none">
              <span class="text-decoration-none fw_normal">Go To Awards</span>
              <img src="@/assets/images/arrow-right-blue.svg" class="ms-2" />
            </a>
          </div>
        </div>
      </div>

      <div class="col-md-12 col-lg-4 col-md-4 mt-5">
        <div class="p-4">
          <a href="#" class="text-primary text-decoration-none fw_normal"> Our Acheivement </a>

          <h2 class="fw-bold mt-2 ">We are Connecting You The Digital Life.</h2>
          <p class="text_gray mt-3">
            The scope the Social Media becomes crucial Is helps the business to directly engage with
            their needs and wants.
          </p>

          <button class="btn btn-primary text-white mt-4">
            <span class="self-center">Discover me</span>
            <img src="@/assets/images/arrow-right.svg" class="self-center ps-2" />
          </button>
        </div>
      </div>
    </div>
  </div>
  <!-- Digital life ending -->

  <!-- Active Member -->
  <div class="container py-5 mt-3">

    <div class="row justify-content-center ">
      <div class="col-lg-4 col-md-8 col-sm-12 col-xs-12">
        <div class="text-center">
          <a href="#" class="text-decoration-none fw_normal">
            Valuable Team
          </a>

          <h2 class="fw-bold ">Our Active Members</h2>
          <p class="text_gray mt-2">
            when an unknown printer took a galley of type and meeting fari scrambled it.
          </p>


          <div
            class=" p-2 radius_default bg-primary bg-opacity-10 d-flex flex-column flex-sm-row justify-content-between ">
            <button @click="state.active_tab = 'one'" class="btn fw_normal mx-1 " :class="state.active_tab === 'one'
              ? 'btn-primary text-white'
              : ''
              ">
              Newst
            </button>
            <button @click="state.active_tab = 'two'" class="btn fw_normal mx-1 " :class="state.active_tab === 'two'
              ? 'btn-primary text-white'
              : ''
              ">
              Popular
            </button>
            <button @click="state.active_tab = 'three'" class="btn fw_normal mx-1" :class="state.active_tab === 'three'
              ? 'btn-primary text-white'
              : ''
              ">
              Active
            </button>
          </div>
        </div>
      </div>
    </div>



    <div class="row pb-5">
      <div class="col-md-12 col-lg-3 mt-5">
        <div class="px-3 py-4 border rounded-4 user_box text-center">
          <img src="@/assets/images/user_one.svg" class="img-fluid mx-auto" />

          <h3 class="text-xl font-semibold">Fahim Rahman</h3>
          <p class="text_gray mb-0">@rahman</p>
        </div>

      </div>
      <div class="col-md-12 col-lg-3 mt-5">
        <div class="px-3 py-4 border rounded-4 user_box text-center">
          <img src="@/assets/images/user_two.svg" class="img-fluid mx-auto" />

          <h3 class="text-xl font-semibold">Kazi Rehman</h3>
          <p class="text_gray mb-0">@Rahman</p>
        </div>

      </div>
      <div class="col-md-12 col-lg-3 mt-5">
        <div class="px-3 py-4 border rounded-4 user_box text-center">
          <img src="@/assets/images/user_three.svg" class="img-fluid mx-auto" />

          <h3 class="text-xl font-semibold">Masterero Ali</h3>
          <p class="text_gray mb-0">@Master</p>
        </div>
      </div>

      <div class="col-md-12 col-lg-3 mt-5">

        <div class="px-3 py-4 border rounded-4 user_box text-center">
          <img src="@/assets/images/user_four.svg" class="img-fluid mx-auto" />

          <h3 class="text-xl font-semibold">Alia Karon</h3>
          <p class="text_gray mb-0">@Alia</p>
        </div>

      </div>
    </div>
  </div>
  <!-- End Active Member -->

  <!-- Footer -->
  <div class="bg-footer">
    <div class="container">
      <div class="row py-5 align-items-center d-flex flex-column flex-sm-row">
        <div class="col-sm-12 col-lg-2 col-lg-2 md:col-span-12 text-center py-2 ">
          <img src="@/assets/images/logo-light.svg" class="self-center mx-auto md:ml-0" />
        </div>

        <div class="col-sm-12 col-lg-2 col-lg-8   row g-1 d-flex flex-column flex-sm-row align-items-center py-2">
          <div class="col text-center">
            <p class="text-white text-center mb-0">Home</p>
          </div>
          <div class="col text-center">
            <p class="text-white text-center mb-0">Resources</p>
          </div>
          <div class="col text-center">
            <p class="text-white text-center mb-0">Community</p>
          </div>
          <div class="col text-center">
            <p class="text-white text-center mb-0">Members</p>
          </div>
        </div>

        <div class="col-sm-12 col-lg-2 col-lg-2  row g-1 d-flex justify-content-end py-2">
          <div class="col text-center">
            <img src="@/assets/images/t.svg" class="self-center object-contain" />
          </div>
          <div class="col text-center">
            <img src="@/assets/images/i.svg" class="self-center object-contain" />
          </div>
          <div class="col text-center">
            <img src="@/assets/images/f.svg" class="self-center object-contain" />
          </div>
          <div class="col text-center">
            <img src="@/assets/images/in.svg" class="self-center object-contain" />
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Footer end -->
</template>
