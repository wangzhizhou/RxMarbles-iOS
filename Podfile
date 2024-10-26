platform :ios, '12.0'
use_frameworks!
target 'RxMarbles' do
  pod 'RxSwift'
  pod 'RxCocoa'
  pod 'Device'
  pod 'RazzleDazzle', :git => 'https://github.com/wangzhizhou/RazzleDazzle.git', :branch => 'master'
end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['SWIFT_VERSION'] = '6.0'
      config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '12.0'
    end
  end
end
