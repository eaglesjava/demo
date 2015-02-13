#选项卡
---

<div class="ui-tab">
    <ul class="ui-tab-nav ui-border-b">
        <li class="current">热门推荐</li>
        <li>全部表情</li>
        <li>表情</li>
    </ul>
    <ul class="ui-tab-content" style="width: 300%;">
        <li>
            <ul class="ui-list ui-list-link ui-border-b">  
                <li>
                    <div class="ui-list-thumb ui-avatar-s">
                       <span style="background-image:url(http://placehold.sinaapp.com/?100*100)"></span>
                    </div>
                    <div class="ui-list-info ui-border-t">
                        <h4 class="ui-nowrap">这是标题，加ui-nowrap可以超出长度截断</h4>
                        <p class="ui-nowrap">这是内容，加ui-nowrap可以超出长度截断</p>
                    </div>
                </li>
                <li>
                    <div class="ui-list-thumb ui-avatar-s">
                        <span  style="background-image:url(http://placehold.sinaapp.com/?100*100)"></span>
                    </div>
                    <div class="ui-list-info ui-border-t">
                        <h4 class="ui-nowrap">这是标题，加ui-nowrap可以超出长度截断</h4>
                        <p class="ui-nowrap">这是内容，加ui-nowrap可以超出长度截断</p>
                  </div>
                </li>
                <li>
                    <div class="ui-list-thumb ui-avatar-s">
                        <span  style="background-image:url(http://placehold.sinaapp.com/?100*100)"></span>
                    </div>
                    <div class="ui-list-info ui-border-t">
                        <h4 class="ui-nowrap">这是标题，加ui-nowrap可以超出长度截断</h4>
                        <p class="ui-nowrap">这是内容，加ui-nowrap可以超出长度截断</p>
                  </div>
                </li>
                <li>
                    <div class="ui-list-thumb ui-avatar-s">
                        <span  style="background-image:url(http://placehold.sinaapp.com/?100*100)"></span>
                    </div>
                    <div class="ui-list-info ui-border-t">
                        <h4 class="ui-nowrap">这是标题，加ui-nowrap可以超出长度截断</h4>
                        <p class="ui-nowrap">这是内容，加ui-nowrap可以超出长度截断</p>
                  </div>
                </li>
                <li>
                    <div class="ui-list-thumb ui-avatar-s">
                        <span  style="background-image:url(http://placehold.sinaapp.com/?100*100)"></span>
                    </div>
                    <div class="ui-list-info ui-border-t">
                        <h4 class="ui-nowrap">这是标题，加ui-nowrap可以超出长度截断</h4>
                        <p class="ui-nowrap">这是内容，加ui-nowrap可以超出长度截断</p>
                  </div>
                </li>
                <li>
                    <div class="ui-list-thumb ui-avatar-s">
                        <span  style="background-image:url(http://placehold.sinaapp.com/?100*100)"></span>
                    </div>
                    <div class="ui-list-info ui-border-t">
                        <h4 class="ui-nowrap">这是标题，加ui-nowrap可以超出长度截断</h4>
                        <p class="ui-nowrap">这是内容，加ui-nowrap可以超出长度截断</p>
                  </div>
                </li>
                <li>
                    <div class="ui-list-thumb ui-avatar-s">
                        <span  style="background-image:url(http://placehold.sinaapp.com/?100*100)"></span>
                    </div>
                    <div class="ui-list-info ui-border-t">
                        <h4 class="ui-nowrap">这是标题，加ui-nowrap可以超出长度截断</h4>
                        <p class="ui-nowrap">这是内容，加ui-nowrap可以超出长度截断</p>
                  </div>
                </li>
            </ul>
            <div class="ui-loading-wrap">
                <p>加载中</p>
                <i class="ui-loading"></i>
            </div>
        </li>
        <li>
            <ul class="ui-list ui-list-text ui-border-b">
                <li class="ui-border-t">
                    <div class="ui-list-info">
                        <h4 class="ui-nowrap">这是标题，加ui-nowrap可以超出长度截断</h4>
                    </div>
                    <div class="ui-badge">123</div>
                </li>
                <li class="ui-border-t">
                    <div class="ui-list-info">
                        <h4 class="ui-nowrap">这是标题，加ui-nowrap可以超出长度截断</h4>
                    </div>
                    <div class="ui-badge-muted">123</div>
                </li>
                <li class="ui-border-t">
                    <div class="ui-list-info">
                       <h4>标题标题标题标题标题标题标</h4>
                    </div>
                    <div class="ui-list-action">使用中</div>
                </li>
            </ul>
        </li>
        <li>
            <ul class="ui-list ui-list-link ui-border-b">
                <li class="ui-border-t">
                    <div class="ui-list-img">
                        <span style="background-image:url(http://placehold.sinaapp.com/?200*136)"></span>
                    </div>
                    <div class="ui-list-info">
                        <h4 class="ui-nowrap">这是标题，加ui-nowrap可以超出长度截断</h4>
                        <p class="ui-nowrap">这是内容，加ui-nowrap可以超出长度截断</p>
                    </div>
                </li>
                <li class="ui-border-t">
                    <div class="ui-list-img">
                       <span style="background-image:url(http://placehold.sinaapp.com/?200*136)"></span>
                    </div>
                    <div class="ui-list-info">
                        <h4 class="ui-nowrap">这是标题，加ui-nowrap可以超出长度截断</h4>
                    </div>
                </li>
            </ul>
        </li>
    </ul>
</div>
<script>
var tab = new fz.Scroll('.ui-tab', {
    role: 'tab',
    interval: 3000
    //autoplay: true
});
tab.currentPage = 1;
$(tab.nav.children[0]).removeClass('current');
$(tab.nav.children[tab.currentPage]).addClass('current');
tab.scrollTo(-tab.itemWidth*tab.currentPage,0);
tab.on('beforeScrollStart', function(fromIndex, toIndex) {
    console.log(fromIndex, toIndex)
});

tab.on('scrollEnd', function() {
    console.log('end')
});  
</script>
