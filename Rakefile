require 'xcjobs'

def destinations
  [ 'name=iPhone 5s,OS=8.1' ]
end

XCJobs::Test.new('test:ios') do |t|
  t.workspace = 'SwiftGif'
  t.scheme = 'SwiftGif'
  t.configuration = 'Debug'
  t.build_dir = 'build'
  destinations.each do |destination|
    t.add_destination(destination)
  end
  t.formatter = 'xcpretty -c'
end
