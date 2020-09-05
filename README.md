### Hi there 👋
const axios = require('axios')//

module.exports = function (api) {//
 api.loadSource(async actions => {//
    const { data } = await axios.get('http://localhost:1337/events/')//

    const collection = actions.addCollection({ // Object - array of objects or table - in GraphQL
      typeName: 'Event'
    })
 }//
