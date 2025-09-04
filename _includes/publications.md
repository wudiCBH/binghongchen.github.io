<h2 id="research" style="margin: 2px 0px -15px;">Research Experiences</h2>

<div class="publications">
<ol class="bibliography">

{% for item in site.data.research.main %}

<li>
<div class="pub-row row align-items-start mb-3"> <!-- 使用 row 并对齐顶部 -->

  <!-- 左边展示gif -->
  <div class="col-12 col-md-3 mb-2 mb-md-0"> <!-- 手机端占满宽度，桌面端占3/12 -->
    {% if item.image %}
    <img src="{{ item.image }}" class="img-fluid rounded z-depth-1" style="width:100%; height:auto;">
    {% endif %}
  </div>

  <!-- 右边文字部分 -->
  <div class="col-12 col-md-9">
    <!-- 蓝色小字标题 -->
    <div class="title text-primary fw-bold mb-1" style="font-size:14px;">
      {{ item.title }}
    </div>
    <!-- 时间和supervisor -->
    <div class="meta text-muted small mb-1" style="font-size:12px;">
      {{ item.time }} &nbsp; | &nbsp; Supervisor: {{ item.supervisor }}
    </div>
    <!-- 两行描述 -->
    <div class="description" style="font-size:14px;">
      <p style="margin:2px 0;">{{ item.description1 }}</p>
      <p style="margin:2px 0;">{{ item.description2 }}</p>
    </div>
  </div>

</div>
</li>
<br>

{% endfor %}

</ol>
</div>
