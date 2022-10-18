<template >
    <aside class="sidebar-wrapper " :class="`${IsExpanded ? 'sidebar-wrapper-toggle' : ''}`">
        <div class="logo">
            <img src="../assets/logo.svg" alt="Firebase">
        </div>
        <div class="menu-Toggle-wrap ">
            <button class="menu-toggle" @click="ToggleButton">
                <svg viewBox="0 0 24 24" preserveAspectRatio="xMidYMid meet" focusable="false"
                    class="style-scope yt-icon"
                    style="pointer-events: none; display: block; width: 100%; height: 100%;">
                    <g class="style-scope yt-icon">
                        <path d="M21,6H3V5h18V6z M21,11H3v1h18V11z M21,17H3v1h18V17z" class="style-scope yt-icon">
                        </path>
                    </g>
                </svg>
            </button>

        </div>

        <div class="menu">
            <router-link to="/" class="button">
                <div class="icon">
                    <svg viewBox="0 0 24 24" preserveAspectRatio="xMidYMid meet" focusable="false"
                        class="style-scope yt-icon"
                        style="pointer-events: none; display: block; width: 100%; height: 100%;">
                        <g class="style-scope yt-icon">
                            <path d="M4,10V21h6V15h4v6h6V10L12,3Z" class="style-scope yt-icon"></path>
                        </g>
                    </svg>
                </div>
                <span class="text">
                    Home
                </span>
            </router-link>
            <router-link to="/about" class="button">
                <div class="icon">
                    <svg viewBox="0 0 24 24" preserveAspectRatio="xMidYMid meet" focusable="false"
                        class="style-scope yt-icon"
                        style="pointer-events: none; display: block; width: 100%; height: 100%;">
                        <g class="style-scope yt-icon">
                            <path
                                d="M9.8,9.8l-3.83,8.23l8.23-3.83l3.83-8.23L9.8,9.8z M13.08,12.77c-0.21,0.29-0.51,0.48-0.86,0.54 c-0.07,0.01-0.15,0.02-0.22,0.02c-0.28,0-0.54-0.08-0.77-0.25c-0.29-0.21-0.48-0.51-0.54-0.86c-0.06-0.35,0.02-0.71,0.23-0.99 c0.21-0.29,0.51-0.48,0.86-0.54c0.35-0.06,0.7,0.02,0.99,0.23c0.29,0.21,0.48,0.51,0.54,0.86C13.37,12.13,13.29,12.48,13.08,12.77z M12,3c4.96,0,9,4.04,9,9s-4.04,9-9,9s-9-4.04-9-9S7.04,3,12,3 M12,2C6.48,2,2,6.48,2,12s4.48,10,10,10s10-4.48,10-10S17.52,2,12,2 L12,2z"
                                class="style-scope yt-icon"></path>
                        </g>
                    </svg>
                </div>
                <span class="text">
                    About
                </span>
            </router-link>
            <router-link to="/shorts" class="button">
                <div class="icon">
                    <svg viewBox="0 0 24 24" preserveAspectRatio="xMidYMid meet" focusable="false"
                        class="style-scope yt-icon"
                        style="pointer-events: none; display: block; width: 100%; height: 100%;">
                        <g height="24" viewBox="0 0 24 24" width="24" class="style-scope yt-icon">
                            <path
                                d="M10 14.65v-5.3L15 12l-5 2.65zm7.77-4.33c-.77-.32-1.2-.5-1.2-.5L18 9.06c1.84-.96 2.53-3.23 1.56-5.06s-3.24-2.53-5.07-1.56L6 6.94c-1.29.68-2.07 2.04-2 3.49.07 1.42.93 2.67 2.22 3.25.03.01 1.2.5 1.2.5L6 14.93c-1.83.97-2.53 3.24-1.56 5.07.97 1.83 3.24 2.53 5.07 1.56l8.5-4.5c1.29-.68 2.06-2.04 1.99-3.49-.07-1.42-.94-2.68-2.23-3.25zm-.23 5.86l-8.5 4.5c-1.34.71-3.01.2-3.72-1.14-.71-1.34-.2-3.01 1.14-3.72l2.04-1.08v-1.21l-.69-.28-1.11-.46c-.99-.41-1.65-1.35-1.7-2.41-.05-1.06.52-2.06 1.46-2.56l8.5-4.5c1.34-.71 3.01-.2 3.72 1.14.71 1.34.2 3.01-1.14 3.72L15.5 9.26v1.21l1.8.74c.99.41 1.65 1.35 1.7 2.41.05 1.06-.52 2.06-1.46 2.56z"
                                class="style-scope yt-icon"></path>
                        </g>
                    </svg>
                </div>
                <span class="text">
                    Shorts
                </span>
            </router-link>
            <router-link to="/subsciption" class="button">
                <div class="icon">
                    <svg viewBox="0 0 24 24" preserveAspectRatio="xMidYMid meet" focusable="false"
                        class="style-scope yt-icon"
                        style="pointer-events: none; display: block; width: 100%; height: 100%;">
                        <g class="style-scope yt-icon">
                            <path
                                d="M10,18v-6l5,3L10,18z M17,3H7v1h10V3z M20,6H4v1h16V6z M22,9H2v12h20V9z M3,10h18v10H3V10z"
                                class="style-scope yt-icon"></path>
                        </g>
                    </svg>
                </div>
                <span class="text">
                    subsciption
                </span>
            </router-link>
        </div>


    </aside>
</template>
<script>
export default {
    data() {
        return {
            IsExpanded: false
        }
    },
    methods: {
        ToggleButton() {
            this.IsExpanded = !this.IsExpanded
        }
    },

}
</script>
<style lang="scss" scoped>





aside {
  --icon-maxidth:2rem;







    display: flex;
    flex-direction: column;
    // align-items: center;
    background-color: var(--dark);
    color: var(--light);
    width: calc(2rem + 32px);
    overflow: hidden;
    min-height: 100vh;
    padding: 0 0 0 0.5rem ;
            transition: 0.2s ease-in-out;


    .logo {
        margin: 1rem 0;

        img {
            width: var(--icon-maxidth);
        }
    }

    .menu-Toggle-wrap {
        margin-bottom: 1rem;

        :only-child {
            width: var(--icon-maxidth);
        }
    }

    .text {
        opacity: 0;
        scale: 0;
        transition:  0.3s ease-in-out;
    }

    .menu {
        .button {
            display: flex;
            align-items: center;
            text-decoration: none;
            transition: 0.2s ease-in-out;
            padding: 0.5rem 0;
                                                            
            .icon {
                 max-width: var(--icon-maxidth);
                 
            }

            .text {
                flex: 1 1 0 ;
                text-align: center;
                color: wheat;
            }
        }
    }
}

.sidebar-wrapper-toggle {
    width: var(--sidebar-width);

    .menu {

        .button {

            .icon{
                max-width: var(--icon-maxidth);
            }

            .text {
                opacity: 1;
                scale: 1;
            }
        }
    }

}
</style>