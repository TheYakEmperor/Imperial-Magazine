---
layout: /src/layouts/BaseLayoutNoAuthor.astro
title: "Solid Gold Chartbusters";

const allPosts = await Astro.glob('./article/*/*.md');
---
<ul>
{allPosts.map((post) => <li><a href={post.url}>{post.frontmatter.title}</a></li>)}
</ul>