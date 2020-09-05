### Hi there 👋

-import vue from 'vue'
=import react from 'react'
import express from 'express'
import mongoose from 'mongoose'
import Vuetify from 'vuetify'
import materialud from '@material-ui/core'
const axios = require('axios')

module.exports = function (api) {
 api.loadSource(async actions => {
    const { data } = await axios.get('http://localhost:1337/events/')

    const collection = actions.addCollection({ // Object - array of objects or table - in GraphQL
      typeName: 'Event'
    })
 }
