workspace 'GRDBTest'
use_frameworks!
install! 'cocoapods', :deterministic_uuids => false, :warn_for_multiple_pod_sources => false

abstract_target :main do
  project 'GRDBTest'

  pod 'SQLCipher', '4.4.3', :inhibit_warnings => true, :modular_headers => true
  pod 'GRDB.swift/SQLCipher', :git => 'git@github.com:groue/GRDB.swift.git'

  target 'GRDBTest' do
    inherit! :complete
    platform :ios, '14.1'

    target 'GRDBTestTests' do
      inherit! :complete
    end
  end

  target 'WatchOS' do
    inherit! :complete
    platform :watchos, '7.0'    
  end
end
