
<script>
import DefaultLayout from '@/layouts/DefaultLayout' // eslint-disable-line no-unused-vars
import Menu from '@/components/Menu.vue'

export default {
  name: 'TemasView',
  components: {
    Menu
  },
  render (h) {
    let event = this.$route.params.event
    if(!event) {
      this.$router.push({ name:'Home'})
    } else {
      return
        <DefaultLayout>
          <section slot="content">
            <div class="row">
              <div class="col m-1" md="4" v-for="(temas,index) in event.temas" :key="index">
                <p>{tema.nombre}</p>
              </div>
            </div>
          </section>
        </DefaultLayout>
    }
  }
}
</script>