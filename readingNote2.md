# React: Component Lifecycle Events
    by
Joshua Blankenship

  ## What are component lifecycle events?
  *React lets you define components as classes or functions. The methods that you are able to use on these are called lifecycle events. These methods can be called during the lifecycle of a component, and they allow you to update the UI and application states.*

 ## Mounting
  *When an instance of a component is being created and inserted into the DOM it occurs during the mounting phase. Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount all occur in this order during mounting.*

  ## Updating
  *Anytime a component is updated or state changes then it is rerendered. These lifecycle events happen during updating in this order.*

 ## Unmounting
  *The final phase of the lifecycle if called when a component is being removed from the DOM. componentWillUnmount is the only lifecycle event during this phase.*

  ## constructor()
  **constructor(props)**
  *The constructor for a React component is called before it is mounted. When implementing the constructor for a React.Component subclass, you should call super(props) before any other statement. Otherwise, this.props will be undefined in the constructor, which can lead to bugs.*
  
  **Typically, in React constructors are only used for two purposes:**

  - *Initializing local state by assigning an object to this.state.*
  - *Binding event handler methods to an instance.*

  ***constructor(props) {
  super(props);
  // Don't call this.setState() here!
  this.state = { counter: 0 };
  this.handleClick = this.handleClick.bind(this);
}***

## Installation of bootstrap

The best way to consume React-Bootstrap is via the npm package which you can install with npm (or yarn if you prefer).

If you plan on customizing the Bootstrap Sass files, or don't want to use a CDN for the stylesheet, it may be helpful to install vanilla Bootstrap as well.

## Handling Events
  *Handling events with React elements is very similar to handling events on DOM elements. There are some syntax differences:*

  *React events are named using camelCase, rather than lowercase.
  With JSX you pass a function as the event handler, rather than a string.*

 ## <button onClick={activateLasers}>
  Activate Lasers
</button>

## function Form() {
  function handleSubmit(e) {
    e.preventDefault();
    console.log('You clicked submit.');
  }

  return (
    <form onSubmit={handleSubmit}>
      <button type="submit">Submit</button>
    </form>
  );
}

## class Toggle extends React.Component {
  constructor(props) {
    super(props);
    this.state = {isToggleOn: true};

    // This binding is necessary to make `this` work in the callback
    this.handleClick = this.handleClick.bind(this);
  }

  handleClick() {
    this.setState(prevState => ({
      isToggleOn: !prevState.isToggleOn
    }));
  }

  render() {
    return (
      <button onClick={this.handleClick}>
        {this.state.isToggleOn ? 'ON' : 'OFF'}
      </button>
    );
  }
}

ReactDOM.render(
  <Toggle />,
  document.getElementById('root')
);

 [My Readme file page](README.MD)