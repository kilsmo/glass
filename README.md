# glass

Glass is a framework for developing web applications.

The initial idea was to create a framework that made it very easy to handle layout, animations, and drag & drop, and add it on top of established frameworks like React.

The idea has since then morphed into something different. Glass still has the goal to make it very easy to do layout, animations, and drag & drop, but now it is a framework on its own, that does not depend on any other framework.

How is Glass different? One thing is that Glass does not use or need a virtual DOM. Another thing is that the basic idea is not to render a state, but to act on mutations (streams). A component can for example get a mutation that tells it is time to append a new child to the component, the component will then be responsible for create DOM objects for that child component.

Working on mutations instead of state/props is easier when trying to create animations, and doing drag & drop. I find the idea interesting enough to explore, I have been a huge fan of state renderers, but shifting focus to mutations could be a good base for web applications too.

Some possible components:

* Box (The base class component)
* CBox (content box)
* PBox (parent box, has children, layouts children, animates children, handles drag&drop for children, handles child events)
* XBox (A PBox where children are layered inside a row)
* YBox (A PBox where children are layered inside a column)
* SBox (A switch box, that switches between different "pages")
* FBox (A flex box, a box that will stretch to use all unused space in a PBox)
