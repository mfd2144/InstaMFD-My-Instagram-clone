# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'

target 'InstaMFD' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!


pod 'Firebase/Firestore'
pod 'Firebase/Auth'
pod 'Firebase/Storage' 
pod 'FBSDKLoginKit' 


  # Pods for InstaMFD

  target 'InstaMFDTests' do
    inherit! :search_paths
    # Pods for testing
  end

end
post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings.delete 'IPHONEOS_DEPLOYMENT_TARGET'
    end
  end
end

