<template>
  <q-page padding class="text-center">
    <img
      alt="Reigikai logo"
      src="~assets/reigikai-logo.png"
      style="width: 250px; height: 75px; vertical-align: middle"
    />

    <div class="my-font">
      <div class="q-px-sm q-pt-sm q-mb-sm">
        <div class="text-subtitle">
          Shotokan Karate-do Club - SKIF Las Vegas
        </div>
      </div>
    </div>

    <h5 class="my-font">
      Develop Character Through the Study of Shotokan Karate-do<br />
    </h5>
    <h5 class="my-font">
      Reigikai Shotokan Karate-do Club is a Family-Oriented & Not-for-Profit
      Karate Group<br />
    </h5>
    <h5 class="my-font">Participants will learn:</h5>
    <h6 class="my-font">
      Self-Discipline <br />Good Moral Character <br />Self-Defense
      <br />Integrity <br />Perseverance <br />Authentic Traditional Japanese
      Karate
    </h6>

    <div class="my-font">
      <div class="q-pa-md">
        <q-markup-table>
          <thead>
            <tr>
              <th class="text-left">Class Schedule</th>
              <th class="text-right">Time</th>
              <th class="text-right">Rank/Age</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td class="text-left">Monday</td>
              <td class="text-right">5:30pm - 6:30pm<br /></td>
              <td class="text-right">Beginners<br />(Kids, Teens, Adults)</td>
            </tr>
            <tr>
              <td class="text-left"></td>
              <td class="text-right">6:30pm - 8:00pm<br /></td>
              <td class="text-right">
                Intermediate, Advanced, and Black Belt<br />(Kids, Teens, Adults)</td>
            </tr>
            <tr>
              <td class="text-left">Wednesday</td>
              <td class="text-right">5:30pm - 6:30pm<br /></td>
              <td class="text-right">Beginners<br/>(Kids, Teens, Adults)</td>
            </tr>
            <tr>
              <td class="text-left"></td>
              <td class="text-right">6:30pm - 8:00pm<br /></td>
              <td class="text-right">
                Intermediate, Advanced, and Black Belt<br />(Kids, Teens, Adults)</td>
            </tr>
            <tr>
              <td class="text-left">Friday</td>
              <td class="text-right">7:30pm - 8:30pm</td>
              <td class="text-right">Kumite Training<br>(Kids, Teens, Adults)</td>
            </tr>

            <tr>
              <td class="text-left">Saturday</td>
              <td class="text-right">9:30am - 10:30am</td>
              <td class="text-right">
                Advanced Kata Training<br />(Intermediate, Advanced, and Black Belt)</td>
            </tr>
            <tr>
              <td class="text-left"></td>
              <td class="text-right">10:30am - 11:45am<br></td>
              <td class="text-right">Beginners<br>(Kids, Teens, Adults)</td>
            </tr>
            <tr>
              <td class="text-left"></td>
              <td class="text-right">10:30am - 12:30pm<br></td>
              <td class="text-right">Intermediate, Advanced, and Black Belt<br>(Kids, Teens, Adults)</td>
            </tr>
            <tr>
              <td class="text-left">Sunday</td>
              <td class="text-right">10:30am - 12:30pm</td>
              <td class="text-right">Competition Team Training<br>(Drills, Core Training, Agility/Strength Conditioning)</td>
            </tr>
          </tbody>
        </q-markup-table>
      </div>
    </div>

    <h4 class="my-font">Contact Us</h4>

    <div class="my-font">
      <div class="q-pa-md">
        <q-markup-table>
          <thead>
            <tr>
              <th class="text-left">Instructor</th>
              <th class="text-right">Phone Number</th>
              <th class="text-right">Email</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td class="text-left">Sensei Ronald Tolentino</td>
              <td class="text-right">702-493-5253<br /></td>
              <td class="text-right">702karatedo@gmail.com</td>
            </tr>
            <tr>
              <td class="text-left">Sensei Joseph Tolentino</td>
              <td class="text-right">702-588-3460<br /></td>
              <td class="text-right">joetolentino84@yahoo.com</td>
            </tr>
            <tr>
              <td class="text-left">Sensei Joshua Tolentino</td>
              <td class="text-right">702-324-2752<br /></td>
              <td class="text-right"></td>
            </tr>
            <tr>
              <td class="text-left">Sensei Steven Olivares</td>
              <td class="text-right">702-712-6457<br /></td>
              <td class="text-right"></td>
            </tr>
          </tbody>
        </q-markup-table>
      </div>
    </div>

    <q-page-scroller
      position="bottom-right"
      :scroll-offset="150"
      :offset="[18, 18]"
    >
      <q-btn fab icon="keyboard_arrow_up" color="accent" />
    </q-page-scroller>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "IndexPage",
});
</script>
