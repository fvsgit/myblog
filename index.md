---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
<div class="center-div">
    <form class="center-form">
        <input type="text" placeholder="Search for apps here...">
    </form>
</div>
 
<section class="tiles">
    <ul style="list-style: none;">
        {% for app in site.applications %} 
            <li> 
                <h1>{{ app.name }}</h1>
                <p>{{ app.description }}</p>
                <a href="{{ app.url }}">Link</a>
            </li> 
        {% endfor %} 
    </ul>
</section>
