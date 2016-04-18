platform :ios, '8.0'
use_frameworks!

source 'https://github.com/CocoaPods/Specs.git'
source 'https://github.com/ooyala/ios-sdk-podspecs.git'

abstract_target 'SharedDeps' do
  pod 'AFNetworking'
  pod 'OoyalaSDK'

  target 'InheritSearchPathsBroken' do
    abstract_target 'TestsShared' do
      inherit! :search_paths
      pod 'OCMock'
      target 'InheritSearchPathsBrokenTests'
    end
  end

  target 'InheritSearchPathsBroken WatchKit 1 Extension'
end

