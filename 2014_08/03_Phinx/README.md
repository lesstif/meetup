PHP용 데이터베이스 마이그레이션 툴 Phinx 발견!
==============================================

저는 Codeigniter와 Laravel 이라는 PHP 프레임워크를 사용해보았는데, 둘 다 migration 기능을 제공하고 있습니다. 프레임워크가 제공하는 마이그레이션 기능을 사용하면 데이터베이스의 변경 이력을 남길 수 있고, 롤백이 가능하며, 특히 개발팀이 PHP 코드를 이용하여 데이터베이스 스키마를 쉽게 동기화 할 수 있게 됩니다.

마이그레이션을 통해서 쉽고 안정적으로 데이터베이스를 변경(alter) 할 수 있습니다. 수작업으로 sql을 만들 수도 있지만, 그럴경우 어떤것이 변경되었는지, 다음 배포때는 어떤것이 수행되어야하는지, 기억하고 있어야 합니다.

데이터베이스 테이블 마이그레이션은 어떤 마이그레이션이 수행되었는지 지속적으로 추적해 주기 때문에, 개발자는 단지 프로그램 파일을 업데이트 하고 ```$this->migrate->current()``` 만 호출하면, 배포에 필요한 마이그레이션이 수행됩니다. 현재버전은 ```config/migration.php```에 있습니다.

http://www.cikorea.net/user_guide_2.1.0/libraries/migration.html

프레임워크를 쓰지 않는 레거시 시스템에 사용할 수 있는 데이터베이스 마이그레이션용 라이브러리가 없나 찾아보았는데, 아주 멋진 녀석이 있었네요. Phinx라는 녀석입니다. 사용방법은 Laravel 의 migration 사용법과 비슷하고, 무료입니다~!

관심있으신 분들은 http://phinx.org 로 고고~