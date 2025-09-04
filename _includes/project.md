<h2 id="project" style="margin: 2px 0px -15px;">Project Experiences</h2>

<div class="publications">
<ol class="bibliography">

{% for item in site.data.project.main %}

<li>
<div class="pub-row">
  <!-- 左边展示gif -->
  <div class="col-sm-3 abbr" style="position: relative; padding-right: 15px; padding-left: 15px;">
    {% if item.image %}
    <img src="{{ item.image }}" class="teaser img-fluid z-depth-1" style="width:360px; height:auto;">
    {% endif %}
  </div>

  <!-- 右边文字部分 -->
  <div class="col-sm-9" style="position: relative; padding-right: 15px; padding-left: 20px;">
      <!-- 蓝色小字标题 -->
      <div class="title" style="color:#1e90ff; font-size:14px; font-weight:bold;">
        {{ item.title }}
      </div>
      <!-- 时间和supervisor -->
      <div class="meta" style="font-size:12px; color:gray;">
        {{ item.time }} &nbsp; | &nbsp; {{ item.supervisor }}
      </div>
      <!-- 两行描述 -->
      <div class="description" style="margin-top:5px; font-size:14px;">
        <p>{{ item.description1 }}</p>
        <!-- <p>{{ item.description2 }}</p> -->
      </div>
  </div>
</div>
</li>
<br>

{% endfor %}

</ol>
</div>