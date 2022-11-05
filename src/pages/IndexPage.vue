<template>
  <div>
    <div class="layout-padding">
      <q-chat-message
        v-for="msg in messages"
        :key="msg"
        :label="msg.label"
        :name="msg.name"
        :text="msg.text"
        :stamp="msg.stamp"
        :sent="msg.sent"
        :text-color="msg.textColor"
        :bg-color="msg.bgColor"
      />

      <q-chat-message name="Vladimir">
        <q-spinner-dots size="2rem" />
      </q-chat-message>
    </div>

    <div class="full-width q-pt-md">
      <q-btn
        icon="email"
        class="full-width"
        color="primary"
        label="Teste"
        type="submit"
        outline
        rounded
      />
    </div>
  </div>
</template>

<script>
import { QChatMessage, QSpinnerDots } from "quasar";

export default {
  components: {
    QChatMessage,
    QSpinnerDots,
  },
  data() {
    return {
      message: "",
      messages: [
        {
          label: "Sunday, 19th",
        },
        {
          name: "Vladimir",
          text: ["How are you?"],
          avatar: "statics/boy-avatar.png",
          stamp: "Yesterday 13:34",
        },
        {
          name: "Jane",
          text: ["I'm good, thank you!", "And you?"],
          sent: true,
          textColor: "white",
          bgColor: "black",
          avatar: "statics/linux-avatar.png",
          stamp: "Yesterday at 13:50",
        },
        {
          name: "Jane",
          text: ["And you?"],
          sent: true,
          avatar: "statics/linux-avatar.png",
          stamp: "Yesterday at 13:51",
        },
        {
          label: "Sunday, 19th",
        },
        {
          name: "Vladimir",
          bgColor: "amber",
          textColor: "white",
          text: ["Fine. Nice weather today, right?", "Hmm..."],
          avatar: "statics/boy-avatar.png",
          stamp: "13:55",
        },

        {
          label: "Sunday, 19th",
        },
        {
          name: "Vladimir",
          text: ["How are you?"],
          avatar: "statics/boy-avatar.png",
          stamp: "Yesterday 13:34",
        },
        {
          name: "Jane",
          text: ["I'm good, thank you!", "And you?"],
          sent: true,
          avatar: "statics/linux-avatar.png",
          stamp: "Yesterday at 13:50",
        },
        {
          name: "Jane",
          text: ["And you?"],
          sent: true,
          avatar: "statics/linux-avatar.png",
          stamp: "Yesterday at 13:51",
        },
        {
          label: "Sunday, 19th",
        },
        {
          name: "Vladimir",
          text: ["Fine. Nice weather today, right?", "Hmm..."],
          avatar: "statics/boy-avatar.png",
          stamp: "13:55",
        },

        {
          label: "Sunday, 19th",
        },
        {
          name: "Vladimir",
          text: ["How are you?"],
          avatar: "statics/boy-avatar.png",
          stamp: "Yesterday 13:34",
        },
        {
          name: "Jane",
          text: ["I'm good, thank you!", "And you?"],
          sent: true,
          avatar: "statics/linux-avatar.png",
          stamp: "Yesterday at 13:50",
        },
        {
          name: "Jane",
          text: ["And you?"],
          sent: true,
          avatar: "statics/linux-avatar.png",
          stamp: "Yesterday at 13:51",
        },
        {
          label: "Sunday, 19th",
        },
        {
          name: "Vladimir",
          text: ["Fine. Nice weather today, right?", "Hmm..."],
          avatar: "statics/boy-avatar.png",
          stamp: "13:55",
        },

        {
          label: "Sunday, 19th",
        },
        {
          name: "Vladimir",
          text: ["How are you?"],
          avatar: "statics/boy-avatar.png",
          stamp: "Yesterday 13:34",
        },
        {
          name: "Jane",
          text: ["I'm good, thank you!", "And you?"],
          sent: true,
          avatar: "statics/linux-avatar.png",
          stamp: "Yesterday at 13:50",
        },
        {
          name: "Jane",
          text: ["And you?"],
          sent: true,
          avatar: "statics/linux-avatar.png",
          stamp: "Yesterday at 13:51",
        },
        {
          label: "Sunday, 19th",
        },
        {
          name: "Vladimir",
          text: ["Fine. Nice weather today, right?", "Hmm..."],
          avatar: "statics/boy-avatar.png",
          stamp: "13:55",
        },
      ],
    };
  },
  setup() {
    return {
      mensagens: [
        {
          label: "Sunday, 19th",
        },
      ],
    };
  },
};
</script>
