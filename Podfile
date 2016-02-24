platform :ios, '8.0'
use_frameworks!

abstract_target 'SharedDeps' do
  pod 'AFNetworking'

  target 'InheritSearchPathsBroken' do
    abstract_target 'TestsShared' do
      inherit! :search_paths
      pod 'OCMock'
      target 'InheritSearchPathsBrokenTests'
    end
  end

  target 'InheritSearchPathsBroken WatchKit 1 Extension'
end

