<template>
    <div>
        <video ref="video1" controls autoplay width="340" height="260" poster="http://pic34.nipic.com/20131030/2455348_194508648000_2.jpg" @pause="handlePause" @play="handlePlay">Your browser is too old which doesn't support HTML5 video.</video>
    </div>
</template>
<script>
import flvjs from "flv.js";
export default {
    name: "Video",
    props: {
        types: {
            type: String,
            default: "flv"
        },
        url: {
            types: String,
            default: 'wss://47.98.182.216:8081/live/1.flv'
        }
    },
    data() {
        return {
            flvPlayer: {},
            flvConfig: {
                enableWorker: true,
                enableStashBuffer: false,
                autoCleanupSourceBuffer: true,
                autoCleanupMaxBackwardDuration: 30,
                autoCleanupMinBackwardDuration: 10,
            },
            url2: 'wss://47.98.182.216:8081/live/1.flv'
        };
    },
    beforDertory() {
        for (let k in this.flvPlayer) {
            this.flvPlayer[k].destroy();
        }
        this.flvPlayer = {};
    },
    methods: {
        keepLiveVideo() {
            const video1 = this.$refs.video1;
            this.flvPlayer.video1 = flvjs.createPlayer({
                type: this.types,
                url: this.url,
                isLive: true,
                hasAudio: true,
                hasVideo: true
            }, this.flvConfig);
            this.flvPlayer.video1.attachMediaElement(video1);
            this.flvPlayer.video1.load();

            // const video2 = this.$refs.video2;
            // this.flvPlayer.video2 = flvjs.createPlayer({
            //     type: this.types,
            //     url: this.url,
            //     isLive: true,
            //     hasAudio: true,
            //     hasVideo: true
            // }, this.flvConfig);
            // this.flvPlayer.video2.attachMediaElement(video2);
            // this.flvPlayer.video2.load();

            // const video3 = this.$refs.video3;
            // this.flvPlayer.video3 = flvjs.createPlayer({
            //     type: this.types,
            //     url: this.url,
            //     isLive: true,
            //     hasAudio: true,
            //     hasVideo: true
            // }, this.flvConfig);
            // this.flvPlayer.video3.attachMediaElement(video3);
            // this.flvPlayer.video3.load();

            // const video4 = this.$refs.video4;
            // this.flvPlayer.video4 = flvjs.createPlayer({
            //     type: this.types,
            //     url: this.url,
            //     isLive: true,
            //     hasAudio: true,
            //     hasVideo: true
            // }, this.flvConfig);
            // this.flvPlayer.video4.attachMediaElement(video4);
            // this.flvPlayer.video4.load();

            // const video5 = this.$refs.video5;
            // this.flvPlayer.video5 = flvjs.createPlayer({
            //     type: this.types,
            //     url: this.url,
            //     isLive: true,
            //     hasAudio: true,
            //     hasVideo: true
            // }, this.flvConfig);
            // this.flvPlayer.video5.attachMediaElement(video5);
            // this.flvPlayer.video5.load();

            // const video6 = this.$refs.video6;
            // this.flvPlayer.video6 = flvjs.createPlayer({
            //     type: this.types,
            //     url: this.url,
            //     isLive: true,
            //     hasAudio: true,
            //     hasVideo: true
            // }, this.flvConfig);
            // this.flvPlayer.video6.attachMediaElement(video6);
            // this.flvPlayer.video6.load();
        },
        keepLiveVideo2() {
            const video7 = this.$refs.video7;
            this.flvPlayer.video7 = flvjs.createPlayer({
                type: this.types,
                url: this.url,
                isLive: true,
                hasAudio: true,
                hasVideo: true
            }, this.flvConfig);
            this.flvPlayer.video7.attachMediaElement(video7);
            this.flvPlayer.video7.load();

            const video8 = this.$refs.video8;
            this.flvPlayer.video8 = flvjs.createPlayer({
                type: this.types,
                url: this.url,
                isLive: true,
                hasAudio: true,
                hasVideo: true
            }, this.flvConfig);
            this.flvPlayer.video8.attachMediaElement(video8);
            this.flvPlayer.video8.load();

            const video9 = this.$refs.video9;
            this.flvPlayer.video9 = flvjs.createPlayer({
                type: this.types,
                url: this.url,
                isLive: true,
                hasAudio: true,
                hasVideo: true
            }, this.flvConfig);
            this.flvPlayer.video9.attachMediaElement(video9);
            this.flvPlayer.video9.load();

            const video10 = this.$refs.video10;
            this.flvPlayer.video10 = flvjs.createPlayer({
                type: this.types,
                url: this.url,
                isLive: true,
                hasAudio: true,
                hasVideo: true
            }, this.flvConfig);
            this.flvPlayer.video10.attachMediaElement(video10);
            this.flvPlayer.video10.load();

            const video11 = this.$refs.video11;
            this.flvPlayer.video11 = flvjs.createPlayer({
                type: this.types,
                url: this.url,
                isLive: true,
                hasAudio: true,
                hasVideo: true
            }, this.flvConfig);
            this.flvPlayer.video11.attachMediaElement(video11);
            this.flvPlayer.video11.load();

            const video12 = this.$refs.video12;
            this.flvPlayer.video12 = flvjs.createPlayer({
                type: this.types,
                url: this.url,
                isLive: true,
                hasAudio: true,
                hasVideo: true
            }, this.flvConfig);
            this.flvPlayer.video12.attachMediaElement(video12);
            this.flvPlayer.video12.load();

            const video13 = this.$refs.video13;
            this.flvPlayer.video13 = flvjs.createPlayer({
                type: this.types,
                url: this.url,
                isLive: true,
                hasAudio: true,
                hasVideo: true
            }, this.flvConfig);
            this.flvPlayer.video13.attachMediaElement(video13);
            this.flvPlayer.video13.load();

            const video14 = this.$refs.video14;
            this.flvPlayer.video14 = flvjs.createPlayer({
                type: this.types,
                url: this.url,
                isLive: true,
                hasAudio: true,
                hasVideo: true
            }, this.flvConfig);
            this.flvPlayer.video14.attachMediaElement(video14);
            this.flvPlayer.video14.load();

            const video15 = this.$refs.video15;
            this.flvPlayer.video15 = flvjs.createPlayer({
                type: this.types,
                url: this.url,
                isLive: true,
                hasAudio: true,
                hasVideo: true
            }, this.flvConfig);
            this.flvPlayer.video15.attachMediaElement(video15);
            this.flvPlayer.video15.load();

            const video16 = this.$refs.video16;
            this.flvPlayer.video16 = flvjs.createPlayer({
                type: this.types,
                url: this.url,
                isLive: true,
                hasAudio: true,
                hasVideo: true
            }, this.flvConfig);
            this.flvPlayer.video16.attachMediaElement(video16);
            this.flvPlayer.video16.load();
        },
        stopLiveVideo() {
            for (let k in this.flvPlayer) {
                this.flvPlayer[k].destroy();
            }
            this.flvPlayer = {};
        },
        handlePause() {
            // if (this.flvPlayer) {
            //     this.flvPlayer.destroy();
            //     this.flvPlayer = null;
            // }
        },
        handlePlay() {
            // if (this.flvPlayer == null) {
            //     const video1 = this.$refs.video1;
            //     this.flvPlayer = flvjs.createPlayer({
            //         type: this.types,
            //         url: this.url
            //     });
            //     this.flvPlayer.attachMediaElement(video1);
            //     this.flvPlayer.load();
            // }
        },
    }
};
</script>