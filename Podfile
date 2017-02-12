# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'

target 'CoffeeMapper' do
  # Comment the next line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!

  # Pods for CoffeeMapper
  pod 'Firebase'
  pod 'Firebase/Database'
  pod 'Firebase/Auth'
  pod 'GoogleSignIn'
  pod 'RealmSwift'
  pod 'QuadratTouch', '>= 1.0'
  pod 'HCSStarRatingView', '~> 1.4.4'

  target 'CoffeeMapperTests' do
    inherit! :search_paths
    # Pods for testing
  end

  target 'CoffeeMapperUITests' do
    inherit! :search_paths
    # Pods for testing
  end

end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['SWIFT_VERSION'] = '3.0'
    end
  end
end
