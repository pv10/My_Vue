<template>
  <div class="q-pa-md">
    <q-layout view="lHh lpr lFf" container style="height: 600px" class="shadow-2 rounded-borders">
      <q-header elevated>
        <q-toolbar class="glossy">
          <q-btn flat round dense icon="menu" class="q-mr-sm" />
          <!-- <q-avatar>
            <img src="">
          </q-avatar> -->

          <q-toolbar-title style="text-align: center;">WELCOME TO MY PROFILE</q-toolbar-title>

          <!-- <q-btn flat round dense icon="whatshot" /> -->
        </q-toolbar>
      </q-header>

      <!-- <q-footer elevated>
        <q-toolbar class="glossy">
          <q-toolbar-title>Footer</q-toolbar-title>
        </q-toolbar>
      </q-footer> -->

      <q-page-container>
        <q-page class="q-pa-md">
          <div class="q-col-gutter-md row items-start">
            
              <div class="col-2">
                
                <q-img
                  src="../assets/PujaVerma.jpg"
                  style="max-width: 300px; height: 150px;"
                  :fit="scale-down"
                  img-class="my-custom-image"
                >
                </q-img>
              </div>
            

            <div class="col-7 text-weight-medium text-left my-name" >
              
              <span style="font-size: 40px;">Puja Prakash Verma</span><br>
              Contact:  9370307321
              <br>
              PS No: 10725929
              <br>
              email:    Puja.Verma@ltimindtree.com
              
            </div>
           
          </div>
          <br><br>

            <!-- <div class="q-col-gutter-md row items-start">
               
              <div class="col-4">
                <q-img 
                src="../assets/intrests.jpg">
                  <div class="absolute-full text-subtitle2 flex flex-center">
                  
                  About Me
                  </div>
                  <q-list class="absolute-full transparent">
                  <q-item to="aboutme" class="absolute-full transparent"></q-item>
                  </q-list>
                </q-img>
              </div>
              
            
            
              <div class="col-4">
                <q-img 
                  src="../assets/education2.jpg">
                  <div class="absolute-full text-subtitle2 flex flex-center">
                  Education
                  </div>
                  <q-list class="absolute-full transparent">
                  <q-item to="education" class="absolute-full transparent"></q-item>
                </q-list>
                </q-img>
              </div>

              <div class="col-4">
                <q-img 
                src="../assets/intrests.jpg">
                  <div class="absolute-full text-subtitle2 flex flex-center">
                  Hobbies
                  </div>
                  <q-list class="absolute-full transparent">
                  <q-item to="hobbies" class="absolute-full transparent"></q-item>
                </q-list>
                </q-img>
              </div>
            </div>
            <br><br><br> -->

            <div  class="q-col-gutter-md row items-start details" >
            </div>
            <div class="q-pa-md">
                  <q-carousel
                    arrows
                    animated
                    v-model="slide"
                    height="450px"
                  >
                    <q-carousel-slide name="first" img-src="../assets/PujaEducation1.jpg">
                      <div class="absolute-bottom custom-caption">
                        <div class="text-h4">About Me</div>
                        <div class="text-subtitle1"> Hi!, my name is Puja Prakash Verma <br>
                I'm from Nagpur, and I am a Software Engineer at LTIMindtree.</div>
                      </div>
                    </q-carousel-slide>
                    <q-carousel-slide name="second" img-src="../assets/PujaEducation2.jpg">
                      <div class="absolute-bottom custom-caption">
                        <div class="text-h4">Education</div>
                        <div class="text-subtitle1">Schooling:  Bharti Krishna Vidya Vihar, Nagpur <br>
                          College: Shri Ramdeobaba College of Engineering and Management, Nagpur</div>
                      </div>
                    </q-carousel-slide>
                    <q-carousel-slide name="third" img-src="../assets/PujaIntrests.jpg">
                      <div class="absolute-bottom custom-caption">
                        <div class="text-h4">Interests</div>
                        <div class="text-subtitle1"> I like painting, listening to music and mobile photography.</div>
                      </div>
                    </q-carousel-slide>
                  </q-carousel>
                </div>
        
        </q-page>
      </q-page-container>
    </q-layout>
    
  </div>
  
</template>
<script>
  import { ref } from 'vue'

export default {
  setup () {
    return {
      slide: ref('first')
    }
  }
}

</script>

<style lang="sass">
.my-custom-image
  border-radius: 50%
  
.details
  background-color: rgba(0, 0, 0, 0.7)

.custom-caption
  text-align: center
  padding: 40px
  color: white
  background-color: rgba(0, 0, 0, .3)
  
  
</style>