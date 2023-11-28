# glass

Glass is a framework for developing web applications.

The initial idea was to create a framework that made it very easy to handle layout, animations, and drag & drop, and add it on top of established frameworks like React.

The idea has since then morphed into something different. Glass still has the goal to make it very easy to do layout, animations, and drag & drop, but now it is a framework on its own, that does not depend on any other framework.

How is Glass different? One thing is that Glass does not use or need a virtual DOM. Another thing is that the basic idea is not to render a state, but to act on mutations (streams). A component can for example get a mutation that tells it is time to append a new child to the component, the component will then be responsible for create DOM objects for that child component.

Working on mutations instead of state/props is easier when trying to create animations, and doing drag & drop. I find the idea interesting enough to explore, I have been a huge fan of state renderers, but shifting focus to mutations could be a good base for web applications too.

I plan to create this framework bit by bit, trying to solve one small problem at a time by implementing enough to support a specific example, but not adding more than is needed. The goal is to avoid over-engineering, and hopefully reach a well-designed framework in the end of the process.

