# Accelerator Log

## Options
```json
{
  "apiDescription" : "Customer Service",
  "apiOwner" : "default-team",
  "apiSystem" : "",
  "artifactId" : "customer-profile",
  "bsGitBranch" : "main",
  "bsGitRepository" : "github.com?owner=trisberg&repo=new-java-rest-service",
  "buildTool" : "maven",
  "databaseMigrationTool" : "flyway",
  "databaseName" : "postgres-database",
  "exposeOpenAPIEndpoint" : true,
  "groupId" : "com.example",
  "javaVersion" : "11",
  "liveUpdateIDESupport" : true,
  "packageName" : "com.example.customerprofile",
  "projectName" : "java-rest-service",
  "sourceRepositoryPrefix" : "gcr.io/cf-sandbox-trisberg"
}
```
## Log
```
┏ engine (Chain)
┃  Info Running Chain(GeneratorValidationTransform, UniquePath)
┃ ┏ ┏ engine.transformations[0].validated (Combo)
┃ ┃ ┃  Info Combo running as Let(symbols, in: Chain(chain))
┃ ┃ ┃ engine.transformations[0].validated.chain (Let)
┃ ┃ ┃ Debug Adding symbol packageDirectory with value 'com/example/customerprofile'
┃ ┃ ┃ Debug Adding symbol workloadResourceName with value 'customer-profile'
┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Combo, Combo, Combo, Combo, Combo, Combo, Combo, Combo, Combo, Combo, Combo, Exclude)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#buildTool == 'maven') evaluated to true
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Exclude, Merge(merge), UniquePath(UseLast))
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[0].<combo> (Chain)
┃ ┃ ┃ ┃ ┃  Info Condition (#buildTool == 'maven') evaluated to true
┃ ┃ ┃ ┃ ┃  Info Running Chain(Exclude, Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[0] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**]
┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug build.gradle.kts matched [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.jar matched [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.properties matched [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew matched [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew.bat matched [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug settings.gradle.kts matched [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/V1.0__create_customer_profile_table.sql didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/db.changelog-master.xml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[0].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[0].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/db.changelog-master.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[0].<combo>.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [pom.xml, README.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [pom.xml, README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml, README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/V1.0__create_customer_profile_table.sql didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/db.changelog-master.xml didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[1].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[1].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [pom.xml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/V1.0__create_customer_profile_table.sql didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/db.changelog-master.xml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[1].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace [<groupId>com.vmware.tap.accelerators</groupId>-><groupId>com.example...(truncated)]
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[2].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[2].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [README.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/V1.0__create_customer_profile_table.sql didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/db.changelog-master.xml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[2].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace regex '--- StartGradle[\s\S]+?--- EndGradle' with ''
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[2].<combo>.transformations[2] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗  Info Will replace regex '--- StartMaven\s|--- EndMaven\s' with ''
┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[2] (UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[1] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#buildTool == 'gradle') evaluated to false
┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#databaseMigrationTool == 'flyway') evaluated to true
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Exclude, Merge(merge), UniquePath(UseLast))
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[2].<combo> (Chain)
┃ ┃ ┃ ┃ ┃  Info Condition (#databaseMigrationTool == 'flyway') evaluated to true
┃ ┃ ┃ ┃ ┃  Info Running Chain(Exclude, Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[0] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [src/main/resources/db/changelog/**]
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/db.changelog-master.xml matched [src/main/resources/db/changelog/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/V1.0__create_customer_profile_table.sql matched [src/main/resources/db/changelog/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┗ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[0].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[0].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug .gradle/7.5/executionHistory/executionHistory.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[0].<combo>.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [pom.xml, build.gradle.kts, **/application.properties]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties matched [pom.xml, build.gradle.kts, **/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [pom.xml, build.gradle.kts, **/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml, build.gradle.kts, **/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[1].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[1].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [pom.xml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[1].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace regex '<dependency>\s+<groupId>org\.liquibase</groupId>\s+<artifactId>liquibase-core</artifactId>\s+</dependency>\s+' with ''
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[2].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[2].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [build.gradle.kts]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[2].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace [    implementation("org.liquibase:liquibase-core")->]
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[3] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[3].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, OpenRewriteRecipe, OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[3].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**/application.properties]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties matched [**/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ╺ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[3].<combo>.transformations[1] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┗ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[3].<combo>.transformations[2] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[2] (UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[3] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#databaseMigrationTool == 'liquibase') evaluated to false
┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseLast))
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[4].merge (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[0].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[0].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug config/workload-api-provider.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[0].<combo>.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml matched [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml matched [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug config/workload-api-provider.yaml matched [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#exposeOpenAPIEndpoint) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[1].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#exposeOpenAPIEndpoint) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[1].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [config/workload-api-provider.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug config/workload-api-provider.yaml matched [config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[1].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#exposeOpenAPIEndpoint) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [DESCRIPTION_VAL->Customer Service, OWNER_VAL->default-team, SYSTEM_VAL->]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[1].<combo>.transformations[2] (RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug Path 'config/workload-api-provider.yaml' matched '^(?<folder>.*/)?(?<filename>([^/]+?|)(?=(?<ext>\.[^/.]*)?)$)' with groups {ext=.yaml, folder=config/, filename=workload-api-provider.yaml, g0=config/workload-api-provider.yaml, g1=config/, g2=workload-api-provider.yaml, g3=workload-api-provider.yaml, g4=.yaml} and was rewritten to 'config/workload.yaml'
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (!#exposeOpenAPIEndpoint) evaluated to false
┃ ┃ ┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[3] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[3].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[3].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [config/workload.yaml, config/test-pipeline.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml matched [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug config/workload-api-provider.yaml didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[3].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [rest-service-db->customer-profile]
┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseFirst))
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[5].merge (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(InvokeFragment, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0] (InvokeFragment)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Let(symbols, in: Chain(Merge(merge), UniquePath(UseLast)))
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge (Let)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Adding symbol workloadJavaVersion with value '11'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[0].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[0].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [pom.xml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug README.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[0].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace regex '<java.version>.*<' with '<java.version>11<'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[1].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[1].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [build.gradle]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug README.md didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[1].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace regex 'sourceCompatibility = .*' with 'sourceCompatibility ...(truncated)'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[2].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[2].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [build.gradle.kts]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug README.md didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[2].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace regex '(?<unmodified>JavaVersion\.VERSION_)(\d+)' with '${unmodified}11'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[3] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[3].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[3].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [config/workload.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [config/workload.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug README.md didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[3].<combo>.transformations[1] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[4] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Exclude, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[4].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Exclude, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[4].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [config/*.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [config/*.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml matched [config/*.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug README.md didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[4].<combo>.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [config/workload.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug config/test-pipeline.yaml didn't match [config/workload.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[4].<combo>.transformations[2] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗  Info Will replace regex '(?<unmodified>image: bellsoft/liberica-openjdk-\w*:)(\d+)' with '${unmodified}11'
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Include
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[1].include (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug .gradle/7.5/executionHistory/executionHistory.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ Debug Multiple representations for path 'pom.xml', will use the one appearing first 
┃ ┃ ┃ ┃ ┗ ┗ Debug Multiple representations for path 'config/test-pipeline.yaml', will use the one appearing first 
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#buildTool == 'maven') evaluated to true
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseFirst))
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[6].merge (Chain)
┃ ┃ ┃ ┃ ┃  Info Condition (#buildTool == 'maven') evaluated to true
┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(InvokeFragment, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0] (InvokeFragment)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseLast))
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#liveUpdateIDESupport) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge.transformations[0].sources[0].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#liveUpdateIDESupport) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge.transformations[0].sources[0].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [Tiltfile]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug Tiltfile matched [Tiltfile] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge.transformations[0].sources[0].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [my-project->customer-profile]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge.transformations[0].sources[0].<combo>.transformations[2] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace [dev.local->gcr.io/cf-sandbox-tr...(truncated)]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#liveUpdateIDESupport) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge.transformations[0].sources[1].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#liveUpdateIDESupport) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge.transformations[0].sources[1].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [DEPLOYING.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md matched [DEPLOYING.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug Tiltfile didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge.transformations[0].sources[1].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [my-project->customer-profile]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge.transformations[0].sources[1].<combo>.transformations[2] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [dev.local->gcr.io/cf-sandbox-tr...(truncated)]
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Include
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[1].include (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug config/test-pipeline.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[7] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseFirst))
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[7].merge (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(InvokeFragment, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[0].sources[0] (InvokeFragment)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[0].sources[0].validated (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[0].sources[0].validated.chain (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Combo, Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[0].sources[0].validated.chain.transformations[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#bsGitRepository != null) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[0].sources[0].validated.chain.transformations[0].chain (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#bsGitRepository != null) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[0].sources[0].validated.chain.transformations[0].chain.transformations[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Let(symbols, in: Chain(Include, chain...))
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[0].sources[0].validated.chain.transformations[0].chain.transformations[0].<combo> (Let)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Adding symbol repoUrl with value 'https://github.com?owner=trisberg&repo=new-java-rest-service'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[0].sources[0].validated.chain.transformations[0].chain.transformations[0].<combo>.in (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, OpenRewriteRecipe, ReplaceText, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[0].sources[0].validated.chain.transformations[0].chain.transformations[0].<combo>.in.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**/workload.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [**/workload.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug README.md didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ╺ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[0].sources[0].validated.chain.transformations[0].chain.transformations[0].<combo>.in.transformations[1] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[0].sources[0].validated.chain.transformations[0].chain.transformations[0].<combo>.in.transformations[2] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace regex '(?<beforeBranch>[\s\S]+)(?<branch>branch: [\S]+)(?<rest>[\S\s]*)' with '${beforeBranch}branc...(truncated)'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[0].sources[0].validated.chain.transformations[0].chain.transformations[0].<combo>.in.transformations[3] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗ ┗  Info Will replace regex '(?<beforeSubPath>[\s\S]+)(?<subPath>subPath: [\S]+)(?<rest>[\S\s]*)' with '${beforeSubPath}${re...(truncated)'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[0].sources[0].validated.chain.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#bsGitRepository == null) evaluated to false
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗ null ()
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Include
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[0].sources[1].include (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug .gradle/7.5/executionHistory/executionHistory.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┗ ┗ Debug Multiple representations for path 'config/workload.yaml', will use the one appearing first 
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseFirst))
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[8].merge (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(InvokeFragment, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0] (InvokeFragment)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Let(symbols, in: Chain(Merge(merge), UniquePath(UseLast)))
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge (Let)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Adding symbol databaseResourceName with value 'postgres-database'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo, Combo, Combo, Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Include
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[0].include (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [docker-compose-postgresql.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml matched [docker-compose-postgresql.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/resources/application-test.properties didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[1].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Combo, OpenRewriteRecipe, OpenRewriteRecipe, OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[1].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**/src/main/resources/application-local.properties]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties matched [**/src/main/resources/application-local.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/resources/application-test.properties didn't match [**/src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[1].<combo>.transformations[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(FavorForeign))
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[1].<combo>.transformations[1].merge (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[1].<combo>.transformations[1].merge.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[1].<combo>.transformations[1].merge.transformations[0].sources[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ null ()
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[1].<combo>.transformations[1].merge.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ╺ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[1].<combo>.transformations[2] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ╺ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[1].<combo>.transformations[3] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[1].<combo>.transformations[4] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[2].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Combo, OpenRewriteRecipe, OpenRewriteRecipe, OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[2].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**/src/test/resources/application-test.properties]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [**/src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/resources/application-test.properties matched [**/src/test/resources/application-test.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[2].<combo>.transformations[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(FavorForeign))
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[2].<combo>.transformations[1].merge (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[2].<combo>.transformations[1].merge.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[2].<combo>.transformations[1].merge.transformations[0].sources[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ null ()
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[2].<combo>.transformations[1].merge.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ╺ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[2].<combo>.transformations[2] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ╺ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[2].<combo>.transformations[3] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[2].<combo>.transformations[4] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[3] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[3].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[3].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**/workload.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [**/workload.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/resources/application-test.properties didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[3].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [postgres-database->postgres-database]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[3].<combo>.transformations[2] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[4] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[4].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[4].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [config/postgres.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml matched [config/postgres.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/resources/application-test.properties didn't match [config/postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[4].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [postgres-database->postgres-database]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[4].<combo>.transformations[2] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace [postgresdatabase->postgres-database]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[5] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[5].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[5].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [pom.xml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/resources/application-test.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[5].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace regex '(?<startOfDependencies><dependencies>)(?<existingDependencies>(?![\s\S]+<groupId>org.postgresql</groupId>\s*<artifactId>postgresql</artifactId>[\s\S]+</dependencies>))' with '${startOfDependencie...(truncated)'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[5].<combo>.transformations[2] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace regex '(?<startOfDependencies><dependencies>)(?<existingDependencies>(?![\s\S]+<groupId>org.testcontainers</groupId>\s*<artifactId>postgresql</artifactId>[\s\S]+</dependencies>))' with '${startOfDependencie...(truncated)'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[6] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[6].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[6].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [build.gradle.kts]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/resources/application-test.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[6].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace regex '(?<startOfDependencies>dependencies \{)(?<existingDependencies>(?![\s\S]+implementation\s*\("org.postgresql:postgresql[\s\S]+))' with '${startOfDependencie...(truncated)'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[6].<combo>.transformations[2] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace regex '(?<startOfDependencies>dependencies \{)(?<existingDependencies>(?![\s\S]+testImplementation\s*\("org.testcontainers:postgresql[\s\S]+))' with '${startOfDependencie...(truncated)'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[7] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[7].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Combo, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[7].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [README.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/resources/application-test.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[7].<combo>.transformations[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(FavorForeign))
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[7].<combo>.transformations[1].merge (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[7].<combo>.transformations[1].merge.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[7].<combo>.transformations[1].merge.transformations[0].sources[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ null ()
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[7].<combo>.transformations[1].merge.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[7].<combo>.transformations[2] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will replace regex '(?<existingContent>[\s\S]*)(?<endOfFile>
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info )' with '${existingContent}
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info 
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗  Info ...(truncated)'
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].validated.merge.in.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Include
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[1].include (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug config/workload.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ Debug Multiple representations for path 'README.md', will use the one appearing first 
┃ ┃ ┃ ┃ ┃ ┃ Debug Multiple representations for path 'pom.xml', will use the one appearing first 
┃ ┃ ┃ ┃ ┗ ┗ Debug Multiple representations for path 'config/workload.yaml', will use the one appearing first 
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[9] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseLast))
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[9].merge (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[9].merge.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[9].merge.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[9].merge.transformations[0].sources[0].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[9].merge.transformations[0].sources[0].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**/*.java]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug config/workload.yaml didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[9].merge.transformations[0].sources[0].<combo>.transformations[1] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[9].merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Exclude
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[9].merge.transformations[0].sources[1].exclude (Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [**/*.java]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug config/workload.yaml didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[9].merge.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[10] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseLast))
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[10].merge (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[10].merge.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[10].merge.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Include
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[10].merge.transformations[0].sources[0].include (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**/*.jar]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/api/CustomerProfileController.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/api/CustomerProfileControllerTest.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/data/CustomerProfileRepositoryTest.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/ApplicationTests.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/data/CustomerProfileRepository.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/domain/CustomerProfileServiceTest.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar matched [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileService.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileResponse.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/Application.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/data/CustomerProfileEntity.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileCreateRequest.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[10].merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Exclude, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[10].merge.transformations[0].sources[1].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Exclude, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[10].merge.transformations[0].sources[1].<combo>.transformations[0] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [**/*.jar]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/api/CustomerProfileController.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/api/CustomerProfileControllerTest.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/data/CustomerProfileRepositoryTest.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/ApplicationTests.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/data/CustomerProfileRepository.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/domain/CustomerProfileServiceTest.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar matched [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileService.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileResponse.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/Application.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/data/CustomerProfileEntity.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileCreateRequest.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[10].merge.transformations[0].sources[1].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [rest-service-db->customer-profile]
┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[10].merge.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[11] (Exclude)
┃ ┃ ┃ ┃ ┃  Info Will exclude [manifest.yaml]
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileChanges/last-build.bin didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/buildOutputCleanup.lock didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug bin/main/application.properties didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/api/CustomerProfileController.java didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/api/CustomerProfileControllerTest.java didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/data/CustomerProfileRepositoryTest.java didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.class didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/cache.properties didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/checksums.lock didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/ApplicationTests.java didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/gc.properties didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/md5-checksums.bin didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.class didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.class didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/data/CustomerProfileRepository.java didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/fileHashes/fileHashes.lock didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Get.class didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/V1.0__create_customer_profile_table.sql didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug manifest.yaml matched [manifest.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/checksums/sha1-checksums.bin didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.class didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug .gradle/vcs-1/gc.properties didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.class didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/domain/CustomerProfileServiceTest.java didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/ApplicationTests.class didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.class didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/Application.class didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.class didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/gc.properties didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug bin/main/db/changelog/db.changelog-master.xml didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug .grype.yaml didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.class didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug bin/main/db/migration/V1.0__create_customer_profile_table.sql didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileService.java didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/Application.java didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileResponse.java didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug .gradle/7.5/dependencies-accessors/dependencies-accessors.lock didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug .gradle/buildOutputCleanup/outputFiles.bin didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug bin/test/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest$Create.class didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug bin/main/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.class didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/data/CustomerProfileEntity.java didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileCreateRequest.java didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [manifest.yaml] -> included
┃ ┗ ┗ ┗ ┗ Debug .gradle/7.5/executionHistory/executionHistory.lock didn't match [manifest.yaml] -> included
┗ ╺ engine.transformations[1] (UniquePath)
```
