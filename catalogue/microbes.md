---
layout: default
title: microbe catalogue
categories: photography microscopy
---

# Microbes

Microbes are not a group of animals, but a general group of any organism too
small to be seen with the naked eye. These include organisms from every kingdom
and domain of life: fungi, bacteria, multi-celled animals, protozoa, and more.
Because of the variety, it would be wildly impractical for this section to be
organized in the same catalogue structure as insects and arachnids.

{% assign data = site.data.microbes %}

{% for group in data %}

<h2 id="{{group.id}}">{{group.level}} {{group.name}}</h2>

{% if group.notes %} {{group.notes}} {% endif %}

{% if group.description %}

<h3>Description</h3>
{{group.description}}
{% endif %}

{% assign prefix = group.imgPrefix %} {% assign images = site.static_files
    | where_exp:"file", "file.name contains prefix" %} {% assign captions =
    subject.captions %}

<div
        style="
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            grid-gap: 1rem;
        "
    >
        {% for img in images %}
        <figure
            style="
                grid-column: auto;
                display: flex;
                flex-direction: column;
                align-items: center;
            "
        >
            <a
                target="_blank"
                href="{{img.path}}"
            >
                <div
                    class="image-container"
                    style="background-image: url({{img.path}});"
                >
                    <div class="overlay"></div>
                    <img
                        alt="Click to embiggen"
                        src="/images/embiggen.png"
                    />
                </div>
            </a>
            <figcaption>{{captions[forloop.index0]}}</figcaption>
        </figure>
        {% endfor %}
    </div>
{% endfor %}
