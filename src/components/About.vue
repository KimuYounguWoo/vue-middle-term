<template>
  <div class="bg-green-50 page-section pt-5 -mb-5">
    <!-- RIGHT -->

    
    <!-- .container -->
  </div>
  <!-- .page-section -->

  <div class="bg-green-50 page-section">
    <div class="container">
      <div class="row">
        <div class="col-lg-6 p-4 -mt-9 lg:mt-0">
          <h2 class="title-section text-2xl">

            <span class="marked">기술 및 경험</span>
          </h2>
          <div class="divider"></div>
          <p class="mb-4">
            {{  about[2] }}
          </p>
          <p class="mb-4">
            {{ about[3] }}
          </p>
          <router-link to="/blog" class="btn btn-primary">내 블로그</router-link>
          <router-link to="/projects" class="btn btn-outline ml-2">
            프로젝트
          </router-link>
        </div>
      </div>
    </div>
    
    <!-- .container -->
        <!-- RIGHT -->
        <div class="container">
      <div class="row">
        <div class="col-lg-6 py-3 wow zoomIn">
        </div>

        <div class="col-lg-6 p-4">
          <h2 class="title-section text-2xl">
            All About
            <span class="marked">Myself</span>
          </h2>
          <div class="divider"></div>

          <div>
            <p>
              {{ about[0] }}
            </p>
          </div>

          <div>
            <p>
              {{ about[1] }}
            </p>
          </div>
        </div>
      </div>
    </div>

    <!-- LEFT -->
    <div class="container">
      <div class="row">
        <div class="col-lg-6 p-4 -mt-9 lg:mt-0">
          <h2 class="title-section text-2xl">
            <span class="marked">2019</span>
          </h2>
          <div class="divider"></div>
          <p class="mb-4">
            가천대학교 컴퓨터공학과 입학
          </p>
          <p class="mb-4">
            평소 컴퓨터를 다루는 것에 흥미가 있었고, 컴퓨터공학과를 선택하게 되었습니다.
          </p>
        </div>
      </div>
    </div>
    <!-- RIGHT -->
    <div class="container">
      <div class="row">
        <div class="col-lg-6 py-3 wow zoomIn">
        </div>
        <div class="col-lg-6 p-4">
          <h2 class="title-section text-2xl">
            2020
          </h2>
          <div class="divider"></div>

          <div>
            <p>
              군 복무
            </p>
          </div>

          <div>
            <p>
              군 복무 간, 비록 관련 있는 보직 및 업무를 맡지는 못했지만, 개발자로서의 역량을 키울 수 있는 시간이었습니다.
            </p>
          </div>
        </div>
      </div>
    </div>
    <!-- LEFT -->
    <div class="container">
      <div class="row">
        <div class="col-lg-6 p-4 -mt-9 lg:mt-0">
          <h2 class="title-section text-2xl">
            <span class="marked">2022</span>
          </h2>
          <div class="divider"></div>
          <p class="mb-4">
            복학 후, 프로젝트
          </p>
          <p class="mb-4">
            복학 후, 가천대학교 동기와 함께 프로젝트를 진행하였습니다. 이를 통해, 협업 능력을 키울 수 있었습니다.
          </p>
        </div>
      </div>
    </div>
    <div class="container">
      <div class="row">
        <div class="col-lg-6 py-3 wow zoomIn">
        </div>
        <div class="col-lg-6 p-4">
          <h2 class="title-section text-2xl">
            2023
          </h2>
          <div class="divider"></div>

          <div>
            <p>
              인턴 입사
            </p>
          </div>

          <div>
            <p>
              부트캠프를 통해, 인턴으로 입사하게 되었습니다. 이를 통해, 실무에서의 개발 경험을 쌓을 수 있었습니다.  
            </p>
          </div>
        </div>
      </div>
    </div>
    <!-- LEFT -->
    <div class="container">
      <div class="row">
        <div class="col-lg-6 p-4 -mt-9 lg:mt-0">
          <h2 class="title-section text-2xl">
            <span class="marked">2024</span>
          </h2>
          <div class="divider"></div>
          <p class="mb-4">
            정규직 전환
          </p>
          <p class="mb-4">
            인턴 기간을 거쳐, 정규직으로 전환하게 되었습니다. 이를 통해, 실무에서의 개발 경험을 더욱 쌓을 수 있었습니다.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      scrollPosition: 0,
      about: [
        "저는 웹 및 앱에서 백엔드 개발자로 일하고 있습니다. 주로 Node.js, Express.js, MongoDB, MySQL, Firebase, AWS, Docker 등을 사용하며, 현재는 Microsoft Azure를 사용하여 클라우드 기반의 서비스를 개발하고 있습니다.",
        "저는 문제를 찾는 과정과 그걸 해결하는 과정에서 흥미를 느껴, 개발자를 하게되었습니다. 이러한 성향은 개발을 할 때, 많은 도움이 되었습니다.",
        "저는 가천대학교 컴퓨터공학과를 전공으로 졸업을 하였습니다. 이 곳에서 정말 좋은 사람들을 만나서 좋은 개발자로 성장할 수 있었습니다,",
        "제 개발 목표는 '사용자가 편리하게 사용할 수 있는 서비스'를 만드는 것입니다. 이를 위해, 사용자의 입장에서 생각하고, 사용자가 편리하게 사용할 수 있는 서비스를 만들기 위해 노력하고 있습니다.",
      ],
    };
  },

  methods: {
    handleScroll(e) {
      this.scrollPosition = e.target.scrollTop;

      if (this.scrollPosition > 100) {
        console.log("UP");
      } else {
        console.log("DOWN");
      }
    },
  },
};
</script>

<style></style>
