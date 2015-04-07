default_pattern = [%r{.*.coffee$}]

options = [
  { input: 'assets/javascripts', output: 'src/', patterns: default_pattern }, 
  { input: 'spec/javascripts/websocket_rails', output: 'spec/javascripts/generated', patterns: default_pattern },
  { input: 'spec/javascripts/helpers', patterns: default_pattern }
]

options.each do |option|
  guard :coffeescript, option do
    watch(option[:patterns])
  end
end
