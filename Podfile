platform :ios, '13.0'
use_frameworks!

target 'XCGLoggerNSLoggerConnector' do
  pod 'XCGLogger', '>= 7'
  pod 'NSLogger', '>= 1.9'
end

post_install do |installer|
	installer.pods_project.targets.each do |target|
		target.build_configurations.each do |config|
			config.build_settings['SWIFT_VERSION'] = '5.0'
		end
	end
end
