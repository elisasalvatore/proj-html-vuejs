<template>
    <div class="section-container">
        <div class="section-name">Blog</div>
        <div class="section-title"><b>Latest</b> Post</div>
        <p>When, while the lovely valley teems with vapour around meand the meriand sun strikes the upper surface.</p>

        <div class="posts-container">
            <div class="long-post">

                <div class="long-text-box">
                    <div class="date">
                        April 21, 2019 
                            <span class="dot">&#xb7;</span> 
                        by Paul
                    </div>
                    <div class="title">Amazon gets CCI nod to acquire 49% stake in</div>
                    <div class="paragraph">When, while the lovely valley teems with vapour around meand the meriadian sun strikes the upper</div>
                </div>

                <div class="bt-container">
                    <button>Read More</button>
                </div>
            </div>

            <div class="container-small-posts">
                <div class="box-small-post bg-blue-dark-to-light" v-for="(post, i) in posts" :key="i">
                    <div class="date">{{post.date}}
                        <span class="dot">&#xb7;</span>
                        by {{post.author}}
                    </div>

                    <div class="title">{{post.title}}</div>
                    <div class="paragraph">{{post.paragraph}}</div>

                    <div class="bt-container">
                        <button>Read More</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Blog',
    props: {
        posts: Array,
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/main.scss';
@import '@/style/sectionsHeading.scss';

.section-container {
    
    .posts-container {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 350px;
        font-size: 11px;
        position: relative;
   
        .long-post {
            display: flex;
            width: 600px;
            height: 250px;
            padding: 30px;
            background: url('../assets/images/headway-537308-unsplash-1380x703.jpg');
            // filter: brightness(0.5);
            // background-color: #333;
            // backdrop-filter: brightness(50%);
            background-size: cover;
            background-position: center;
            border-radius: 20px;

            .long-text-box {
                display: flex;
                flex-direction: column;
                justify-content: end;
                align-items: start;
                width: 70%;     
            }
            
            .bt-container {
                display: flex;
                align-items: end;

                button {
                    position: relative;
                    left: 20%;
                }
            }
        }

        .container-small-posts {
            display: flex;
            justify-content: space-between;
            padding: 20px;

           

            .box-small-post {
                display: flex;
                flex-direction: column;
                justify-content: center;
                align-items: start;
                width: 200px;
                height: 300px;
                padding-left: 25px;
                border-radius: 20px;

                &:first-child {
                    margin-right: 30px;
                }

                .title,
                .paragraph {
                    padding: 10px 0;
                }

                button {
                    position: relative;
                    top: 60%
                }
            }
        }

        .date {
            font-weight: 300;
            color: #fff;
        }

        .title {
            text-align: start;
            font-size: 15px;
            font-weight: 600;
            color: #fff;
            margin: 10px 0;
        }

        .paragraph {
            width: 180px;
            font-size: 11px;
            font-weight: 300;
            text-align: start;
            color: #fff;
            // paragrafo con sospensione
            overflow:hidden;
            text-overflow: ellipsis;
            white-space: nowrap;

            // per mostare paragrafo completo quando in hover
            &:hover {
                white-space: unset;
                text-overflow: unset;
            }
        }

        .dot {
            margin: 0 5px;
        }

        .bg-blue-dark-to-light {
            font-size: 12px;
            background-color: $brg-dark-blue,;
            background-image: linear-gradient(
                to top left,
                $brg-blue,
                $brg-dark-blue, 
            );
        }

        button {
            width: 120px;
            height: 30px;
            font-size: 12px;
            font-weight: 300;
            padding: 5px 10px;
            background-color: #fff;
        }
    }
}    
</style>