---
layout: minimal
title: 文章列表
---

<h2 class="text-2xl font-bold mb-6 flex items-center">
                        <div class="w-8 h-8 rounded-full bg-blue-100 flex items-center justify-center text-blue-600 mr-3">
                            <i class="fas fa-file-alt"></i>
                        </div>
                        文章列表
                    </h2>

{%- assign posts = site.posts -%}

{%- if posts.size > 0 -%}
      
      <div class="grid grid-cols-1 gap-6">
      {%- assign date_format = "%Y-%m-%d" -%}
      {%- for post in posts -%}
        {%- if post.categories contains 'article' -%}
        <article class="glassmorphism p-6 card-hover">
          <div class="flex items-center mb-3">
              <span class="text-sm text-gray-500">{{ post.date | date: date_format }}</span>
              <span class="mx-2 text-gray-300">•</span>
              <span class="text-sm text-blue-500">{{ post.tags | join: ", " }}</span>
          </div>
          <h3 class="text-xl font-semibold mb-3">{{ post.title | escape }}</h3>
          <p class="text-gray-600 mb-4">{{ post.excerpt }}</p>
          <div class="flex justify-between items-center">
              <a href="{{ post.url | relative_url }}" class="text-blue-500 hover:text-blue-700 font-medium">阅读更多 →</a>
              <span class="text-sm text-gray-400"><i class="fas fa-eye mr-1"></i> {{ post.views }}</span>
          </div>
      </article>
      {%- endif -%}
      {%- endfor -%}
      </div>

{%- else -%}
  <div class="glassmorphism p-6">
    <p class="text-gray-600">目前还没有文章，敬请期待！</p>
  </div>
{%- endif -%}