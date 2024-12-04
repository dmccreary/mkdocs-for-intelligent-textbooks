# Admonitions

A admonition is a section of text that is seperate from the main flow.
Admonitions are designed to that they can be quickly skipped over
if the user is not concerned with the topic.
Admontions are used to store text such as abstracts, 
note, info, tip, success, question, warning, failure, danger, bug, example and quote.

[mkdocs-materail admonitions documentation](https://squidfunk.github.io/mkdocs-material/reference/admonitions/)

## Use of Admonitions in Intelligent Textbooks

### Showing the Answer

```markdown
#### Definition of Degree of a Node

What is the "degree" of a node in a graph?

<div class="upper-alpha" markdown>
1. The shortest path between two nodes in the graph
2. The total number of edges connected to the node
3. The number of nodes directly reachable from the node
4. The maximum number of edges any node in the graph has
</div>

??? Question "Show Answer"
    The correct answer is **B**. The degree of a node in a 
    graph is the total number of edges connected to that node. 
    For undirected graphs, this includes all edges, while for 
    directed graphs, it can be further classified into in-degree 
    (edges coming into the node) and out-degree (edges going
    out of the node).
```

Rendering:

#### Definition of Degree of a Node

What is the "degree" of a node in a graph?

<div class="upper-alpha" markdown>
1. The shortest path between two nodes in the graph
2. The total number of edges connected to the node
3. The number of nodes directly reachable from the node
4. The maximum number of edges any node in the graph has
</div>

??? Question "Show Answer"
    The correct answer is **B**. The degree of a node in a 
    graph is the total number of edges connected to that node. 
    For undirected graphs, this includes all edges, while for 
    directed graphs, it can be further classified into in-degree 
    (edges coming into the node) and out-degree (edges going
    out of the node).

## Configuration

```yml
markdown_extensions:
  - admonition
```