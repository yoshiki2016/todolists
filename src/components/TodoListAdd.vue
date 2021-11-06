<template>
  <div class="todo-list-top">
    <input type="text" placeholder="タイトル" />
    <select>
      <option
        v-for="statusItem in statusItems"
        :value="statusItem"
        :key="statusItem"
      >
        {{ statusItem }}
      </option>
    </select>
    <button>追加</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      statusItems: ["未着手", "着手", "完了"],
    };
  },
};
</script>
