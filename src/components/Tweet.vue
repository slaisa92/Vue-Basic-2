<script setup>
import ProfileImage from './profileimage.vue'
import User from './User.vue'
import Timestamp from './Timestamp.vue'
import Message from './Message.vue'
import Actions from './Actions.vue'

const props = defineProps ({
        name: String, 
        image: String, 
        handle: String,
        timestamp: String,
        message: String
})

</script>
<template>
    <div class="tweet">
        <ProfileImage :image="props.image"/>
    <div class="body">
      <div class="top">
        <User userData="user" :name="props.name" :handle="props.handle"/>
        <Timestamp :timestamp="props.timestamp"/>
        </div>
        <Message :message="props.message"/>
        <Actions />
    <div>
        <i class="fas fa-ellipsis-h"></i>
    </div>
    </div>
    </div>
    
</template>
<style>
a {
    color: #42b983;
}
</style>