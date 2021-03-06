---
title: Delete Queries
keywords: graql, query, delete
tags: [graql]
summary: "Graql Delete Queries"
sidebar: documentation_sidebar
permalink: /docs/querying-data/delete-queries
folder: docs
---

A delete query will delete things bound to the specified variables for every result of the [match](./match-clause).

To follow along, or experiment further, with the examples given below, please load the *basic-genealogy.gql* file, which can be found in the *examples* directory of the Grakn installation zip, or on [Github](https://github.com/graknlabs/grakn/blob/master/grakn-dist/src/examples/basic-genealogy.gql).


<ul id="profileTabs" class="nav nav-tabs">
    <li class="active"><a href="#shell1" data-toggle="tab">Graql</a></li>
    <li><a href="#java1" data-toggle="tab">Java</a></li>
</ul>

<div class="tab-content">
<div role="tabpanel" class="tab-pane active" id="shell1">
<pre class="language-graql">
<code>
match $x isa person; delete $x;
</code>
</pre>
</div>
<div role="tabpanel" class="tab-pane" id="java1">
<pre class="language-java">
<code>
qb.match(var("x").isa("person")).delete("x").execute();
</code>
</pre>
</div> <!-- tab-pane -->
</div> <!-- tab-content -->
