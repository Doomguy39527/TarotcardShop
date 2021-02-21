<template>
<div class="container">
  <h2>AVAILABLE SHORTLY</h2>  
  <div id="myCarousel" class="carousel slide" data-ride="carousel">
    <!-- Indicators -->
    <ol class="carousel-indicators">
      <li data-target="#myCarousel" data-slide-to="0" class="active"></li>
      <li data-target="#myCarousel" data-slide-to="1"></li>
      <li data-target="#myCarousel" data-slide-to="2"></li>
    </ol>

    <!-- Wrapper for slides -->
    <div class="carousel-inner">
      <div class="item active">
        <img src="https://i.imgur.com/7gAoSush.jpg" alt="Los Angeles" style="100%;">
      </div>

      <div class="item">
        <img src="https://cdn.hipwallpaper.com/i/97/78/a13N0O.jpg" alt="Chicago" style="width:100%;">
      </div>
    
      <div class="item">
        <img src="https://i.pinimg.com/originals/e8/82/2c/e8822cd98582397996d50016f544048c.jpg" alt="New york" style="width:100% ;" >
      </div>
    </div>

    <!-- Left and right controls -->
    <a class="left carousel-control" href="#myCarousel" data-slide="prev">
      <span class="glyphicon glyphicon-chevron-left"></span>
      <span class="sr-only">Previous</span>
    </a>
    <a class="right carousel-control" href="#myCarousel" data-slide="next">
      <span class="glyphicon glyphicon-chevron-right"></span>
      <span class="sr-only">Next</span>
    </a>
  </div>


  <div class="container">
    <h4>
      รายการสินค้า
    </h4>
    <h1>ราคาทั้งหมด = {{ buyClick7 }} บาท</h1>

    <b-button variant="success"  v-on:click="say" @click="CancelAllItem"
      >จ่ายเงิน</b-button
    >

    <b-button variant="danger" @click="CancelAllItem">
      ยกเลิกการซื้อทั้งหมด
    </b-button>
    <div>
      <b-card-group deck>
        <b-card
          id:1
          title="The Chariot"
          img-src="https://upload.wikimedia.org/wikipedia/en/9/9b/RWS_Tarot_07_Chariot.jpg"
          img-alt="Image"
          img-top
        >
          <b-card-text>
            7,000 บาท
          </b-card-text>
          <template #footer>
            <small class="text-muted">
              <b-button variant="outline-success" @click="buyClickI1">
                Buy<b-badge variant="light"
                  >{{ buyClick1
                  }}<span class="sr-only">unread messges</span></b-badge
                >
              </b-button>
              <b-button variant="outline-danger" @click="CancelItem1">
                Cancel
              </b-button></small
            >
          </template>
        </b-card>

        <b-card
          id:2
          title="Death"
          img-src="https://upload.wikimedia.org/wikipedia/en/d/d7/RWS_Tarot_13_Death.jpg"
          img-alt="Image"
          img-top
        >
          <b-card-text>
            13,000 บาท
          </b-card-text>
          <template #footer>
            <small class="text-muted"
              ><b-button variant="outline-success" @click="buyClickI2">
                Buy<b-badge variant="light"
                  >{{ buyClick2
                  }}<span class="sr-only">unread messges</span></b-badge
                >
              </b-button>
              <b-button variant="outline-danger" @click="CancelItem2">
                Cancel
              </b-button></small
            >
          </template>
        </b-card>

        <b-card
          id:3
          title="The Emperor"
          img-src="https://upload.wikimedia.org/wikipedia/en/c/c3/RWS_Tarot_04_Emperor.jpg"
          img-alt="Image"
          img-top
        >
          <b-card-text>
            4,000 บาท
          </b-card-text>
          <template #footer>
            <small class="text-muted"
              ><b-button variant="outline-success" @click="buyClickI3">
                Buy<b-badge variant="light"
                  >{{ buyClick3 }}<span class="sr-only">unread messges</span>
                </b-badge>
              </b-button>
              <b-button variant="outline-danger" @click="CancelItem3">
                Cancel
              </b-button>
            </small>
          </template>
        </b-card>
      </b-card-group>
    </div>
    <div>
      <b-card-group deck>
        <b-card
          id:4
          title="The Hanged Man "
          img-src="https://upload.wikimedia.org/wikipedia/en/2/2b/RWS_Tarot_12_Hanged_Man.jpg"
          img-alt="Image"
          img-top
        >
          <b-card-text>
            12,000 บาท
          </b-card-text>
          <template #footer>
            <small class="text-muted"
              ><b-button variant="outline-success" @click="buyClickI4">
                Buy<b-badge variant="light"
                  >{{ buyClick4
                  }}<span class="sr-only">unread messges</span></b-badge
                >
              </b-button>
              <b-button variant="outline-danger" @click="CancelItem4">
                Cancel
              </b-button></small
            >
          </template>
        </b-card>

        <b-card
          id:5
          title="Judgement"
          img-src="https://upload.wikimedia.org/wikipedia/en/d/dd/RWS_Tarot_20_Judgement.jpg"
          img-alt="Image"
          img-top
        >
          <b-card-text>
            20,000 บาท
          </b-card-text>
          <template #footer>
            <small class="text-muted"
              ><b-button variant="outline-success" @click="buyClickI5">
                Buy<b-badge variant="light"
                  >{{ buyClick5
                  }}<span class="sr-only">unread messges</span></b-badge
                >
              </b-button>
              <b-button variant="outline-danger" @click="CancelItem5">
                Cancel
              </b-button></small
            >
          </template>
        </b-card>
        <b-card
          id:6
          title="The Lovers"
          img-src="https://upload.wikimedia.org/wikipedia/en/d/db/RWS_Tarot_06_Lovers.jpg"
          img-alt="Image"
          img-top
        >
          <b-card-text>
            6,000 บาท
          </b-card-text>
          <template #footer>
            <small class="text-muted"
              ><b-button variant="outline-success" @click="buyClickI6">
                Buy<b-badge variant="light"
                  >{{ buyClick6
                  }}<span class="sr-only">unread messges</span></b-badge
                >
              </b-button>
              <b-button variant="outline-danger" @click="CancelItem6">
                Cancel
              </b-button></small
            >
          </template>
        </b-card>
      </b-card-group>
    </div>
  </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      buyClick1: 0,
      buyClick2: 0,
      buyClick3: 0,
      buyClick4: 0,
      buyClick5: 0,
      buyClick6: 0,
      buyClick7: 0
    };
  },
       methods: {
    say: function() {
      if (this.buyClick7 != 0) {
        alert(
          "ขอบคุณที่ซื้อสินค้า ขอให้โชคจงมมีแด่ท่าน"
        );
      } else if (this.buyClick7 <= 0) {
        alert("กรุณาเลือกสินค้า");
      }
    },
    buyClickI1() {
      this.buyClick1++;
      this.buyClick7 += 7000;
    },
    buyClickI2() {
      this.buyClick2++;
      this.buyClick7 += 13000;
    },
    buyClickI3() {
      this.buyClick3++;
      this.buyClick7 += 4000;
    },
    buyClickI4() {
      this.buyClick4++;
      this.buyClick7 += 12000;
    },
    buyClickI5() {
      this.buyClick5++;
      this.buyClick7 += 20000;
    },
    buyClickI6() {
      this.buyClick6++;
      this.buyClick7 += 6000;
    },
    CancelItem1() {
      if (this.buyClick1 > 0) {
        this.buyClick1--;
        this.buyClick7 -= 7000;
      }
    },
    CancelItem2() {
      if (this.buyClick2 > 0) {
        this.buyClick2--;
        this.buyClick7 -= 13000;
      }
    },
    CancelItem3() {
      if (this.buyClick3 > 0) {
        this.buyClick3--;
        this.buyClick7 -= 4000;
      }
    },
    CancelItem4() {
      if (this.buyClick4 > 0) {
        this.buyClick4--;
        this.buyClick7 -= 12000;
      }
    },
    CancelItem5() {
      if (this.buyClick5 > 0) {
        this.buyClick5--;
        this.buyClick7 -= 20000;
      }
    },
    CancelItem6() {
      if (this.buyClick6 > 0) {
        this.buyClick6--;
        this.buyClick7 -= 6000;
      }
    },
    CancelAllItem() {1
      if (this.buyClick7 > 0) {
        (this.buyClick1 = 0),
          (this.buyClick2 = 0),
          (this.buyClick3 = 0),
          (this.buyClick4 = 0),
          (this.buyClick5 = 0),
          (this.buyClick6 = 0),
          (this.buyClick7 = 0);
      }
    }
  }
};

</script>
