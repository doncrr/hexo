---
title: 即刻短文
date: 2025-08-22 22:53:17
comments: true
aside: false
type: eaasy
---
<style>
/* 页面初始化 */
div#page {
    background: rgba(255,255,255,0);
    border: 0;
    padding: 0;
}

[data-theme=dark] #twikoo .tk-content,
#twikoo .tk-content {
    padding: 0;
    background: rgba(174,207,235,0);
}

.talk_item,
.tk-expand,
.tk-comments-container>.tk-comment,
.tk-submit:nth-child(1){
    background: rgba(174,207,235,0);
    border: 5px dotted #9ed6d6;
    box-shadow: 0 5px 10px rgb(189 189 189 / 10%);
    transition: all .3s ease-in-out;
    border-radius: 15px;
}
.talk_item:hover,
.tk-comments-container>.tk-comment:hover,
.tk-submit:nth-child(1):hover {
    border-color: #afeeee;
}

.tk-submit {
    padding: 20px 10px 0;
}

.tk-comments-container>.tk-comment {
    padding: 15px;
}

/* 页面初始化结束 */

#talk{
    margin-top: 1rem;
}

#talk .loading {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
}

#talk .loading img {
    width: 200px;
}

.talk_item {
    display: flex;
    flex-direction: column;
    padding: 20px;
    margin-bottom: 15px;
}

.avatar {
    margin: 0 !important;
    width: 45px;
    height: 45px;
    border-radius: 10px;
}


.talk_bottom,
.talk_meta {
    display: flex;
    align-items: center;
    width: 100%;
    line-height: 1.5;
}
.talk_bottom{
    justify-content: space-between;
}
.info {
    display: flex;
    flex-direction: column;
    margin-left: 10px;
}
span.talk_nick {
    color: #eeffee;
    font-size: 1.0rem;
}
svg.is-badge.icon {
    width: 15px;
    margin-left: 5px;
    padding-top: 3px;
}
span.talk_date {
    opacity: .6;
    color: #f7f7f7;
    font-size: 0.8rem;
}

.talk_content {
    line-height: 1.5;
    margin-top: 10px;
    color: #eeffee;
}
.zone_imgbox {
    display: flex;
    flex-wrap: wrap;
    --w: calc(25% - 8px);
    gap: 10px;
    margin-top: 5px;
}
.zone_imgbox a {
    display: block;
    border-radius: 12px;
    width: var(--w);
    aspect-ratio: 1/1;
    position: relative;
}

.zone_imgbox img {
    width: 100%;
    height: 100%;
    margin: 0 !important;
    object-fit: cover;
}
/* 底部 */

.talk_bottom {
    opacity: .9;
}
.talk_bottom .icon {
    color: #8aa0e0;
    float: right;
    transition: all .3s;
}

span.talk_tag{
    font-size: 14px;
    color: #D4F2E7
}
.talk_content>a {
    margin: 0 3px;
    color: #ff7d73 !important;
}
.talk_content>a:hover{
    text-decoration: none !important;
    color: #ff5143 !important
}

/* 提醒 */

.limit {
    transition: all .3s ease-in-out;
    color: rgba(76, 73, 72, 0.6);
}

[data-theme=dark] .limit {
    color: rgba(255, 255, 255, 0.5);
}

.limit {
    display: none;
    text-align: center;
    margin-top: 20px;
    color: var(--font-color);
}
@media screen and (max-width: 900px) {
    .zone_imgbox {
        --w: calc(33% - 5px);
    }
    #talk{
        margin: 10px 3px 0
    }
    #post-comment{
        margin: 0 3px
    }
}

@media screen and (max-width: 768px) {
    .zone_imgbox {
        gap: 6px;
    }
    .zone_imgbox {
        --w: calc(50% - 3px);
    }
    span.talk_date {
        font-size: 14px;
        color: #D4F2E7;
    }
}
</style>
