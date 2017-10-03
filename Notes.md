Project start

- layout of project of all the components
  - Search Bar
  - app
  - chart
  - forcastlist

Middleware
  - allow to block pass or modify before they hit a reducer

Redux promise
  - helps with Ajax request

Axios
  - make a get request

Actions to containers

step 1:
import { connect } from 'react-redux';
import { bindActionCreators } from 'redux';
import { fetchWeather } from '../actions/index';

step 2:
function mapDispatchToProps(dispatch) {
  return bindActionCreators({ fetchWeather }, dispatch)
}

step 3:
export default connect(null, mapDispatchToProps)(SearchBar);

step 4:
export default not in class container
