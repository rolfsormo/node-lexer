{exec} = require 'child_process'

task 'build', 'compiles *.coffee to *.js', (options) ->
  exec 'coffee -lcb examples/*.coffee lib/*.coffee', (err, stdout, stderr) ->
    throw err if err
    console.log(stderr) if stderr

task 'clear', 'cleans project', (options) ->
  exec 'rm examples/*.js lib/*.js'
