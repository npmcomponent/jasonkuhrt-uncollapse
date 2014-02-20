*This repository is a mirror of the [component](http://component.io) module [jasonkuhrt/uncollapse](http://github.com/jasonkuhrt/uncollapse). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/jasonkuhrt-uncollapse`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# uncollapse

  CSS utility for undoing css margin collapsing

 - This utility class prevents decendents from margin collapsing
 - The technique is an evolution upon http://stackoverflow.com/questions/1828804/how-do-i-uncollapse-a-margin

## Installation

    $ component install jasonkuhrt/uncollapse

## API

    .uncollapse

  Apply this class on a container having its bounds protruded by its descendents' margin-top/bottom's

## Example

    <!-- Problem -->
    <article>
      <div style="background-color:grey;">
        <h1>Demo</h1>
      </div>
      <div style="background-color:red;">
        <p style="margin:32px;">Oops, notice I don't make my container 64px tall</p>
      </div>
    </article>



    <!-- Solution -->
    <article>
      <div style="background-color:grey;">
        <h1>Demo</h1>
      </div>
      <div class="uncollapse" style="background-color:red;">
        <p style="margin:32px;">Good, I am now 64px tall</p>
      </div>
    </article>

## License

  MIT
