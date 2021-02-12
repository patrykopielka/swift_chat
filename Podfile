platform :ios, '13.0'

target 'SwiftChat' do
  use_frameworks!

  # Pods for SwiftChat
  pod 'CLTypingLabel', '~> 0.4.0'
  pod 'Firebase/Auth'
  pod 'Firebase/Firestore'
  
  post_install do |installer|
    installer.pods_project.targets.each do |target|
      target.build_configurations.each do |config|
        config.build_settings.delete 'IPHONEOS_DEPLOYMENT_TARGET'
      end
    end
  end

end
