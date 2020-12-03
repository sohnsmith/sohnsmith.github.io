# Memoirs Jekyll Theme

[Live Demo](https://wowthemesnet.github.io/jekyll-theme-memoirs/) | [Docs & Download](https://bootstrapstarter.com/bootstrap-templates/jekyll-theme-memoirs/) |  [Buy me a coffee](https://www.wowthemes.net/donate/)

![memoirs](https://bootstrapstarter.com/assets/img/themes/memoirs-jekyll.jpg)


## LIQUID 사용법

// 변수를 선언한다.
{% assign variable = 'test' %}

// 프린트 한다
{{ variable }}

// 인클루드 (_includes 폴더기준으로 시작)
{% include test/test.html %}
{% if variable == 1 %}
  {% include test/test.html %}
{% elsif variable == 2 %}

{% elsif variable == 3 %}

{% else %}

{% endif %}

{% assign test = '1,2,3,4,5,6,7' %}
{% assign pages = test | split:',' %}
// pages = [1, 2, 3, 4, 5, 6, 7] 배열

for (var i = 0; i < pages.length; i += 1) {
  pages[i]
}

for (var page in pages) {
  page = pages[i]
}

{% for page in pages %}
  // 변수를 넘길 수 있다. test.html 페이지 않에서 사용하는 변수는 xxxx이고 xxxx의 값을 page로 넘겨준다.
  {% include test/test.html xxxx=page %}
{% endfor %}

''
https://shopify.github.io/

#### assets -> 자산 (이미지, css, js, font 등)