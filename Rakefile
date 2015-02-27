require 'xcjobs'

def destinations
  [ 'name=iPhone 6,OS=8.3' ]
end

XCJobs::Test.new('test:ios') do |t|
  t.project = 'SwiftGif'
  t.scheme = 'SwiftGif'
  t.configuration = 'Debug'
  t.build_dir = 'build'
  destinations.each do |destination|
    t.add_destination(destination)
  end
  t.formatter = 'xcpretty -c'
end
