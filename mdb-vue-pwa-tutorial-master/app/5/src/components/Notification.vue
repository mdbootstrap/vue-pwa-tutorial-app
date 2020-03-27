<template>
	<mdb-alert
	v-if="isShown"
	:color="availableStatuses[status].color"
	enterAnimation="bounceIn"
	leaveAnimation="slideOutRight"
	>
		<span
			role="img"
			aria-label="emoji"
			>
			{{availableStatuses[status].emoji}}
		</span>
		{{availableStatuses[status].text}}
	</mdb-alert>
</template>

<script>
import { mdbAlert } from 'mdbvue';

export default {
  name: "Notification",
  components: {
    mdbAlert
  },
  props: {
    status: String
  },
  data() {
    return {
      availableStatuses: {
        offline: {
          color: 'danger',
          emoji: '☢️',
          text: 'Offline mode engaged.'
        },
        online: {
          color: 'success',
          emoji: '👌',
          text: 'Back online!'
        }
      },
      isShown: false,
    }
  },
  methods: {
    showAlert() {
      this.isShown = true;
      const timeout = setTimeout(this.hideAlert, 3000);
    },
    hideAlert() {
      this.isShown = false;
    }
  },
  watch: {
    status() {
      this.showAlert();
    }
  }
}
</script>

<style scoped>
	.alert {
		position: absolute;
		z-index: 2;
		right: 0;

	}
	.alert span {
		margin-right: 10px;
	}
</style>
