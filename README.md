# KafkaStream

Use of delegation token:

`export KAFKA_OPTS="-Djava.security.auth.login.config=/home/luoshi/token-jaas-uat.conf -Dlog4j.configuration=/home/luoshi/tools-log4j.properties -Dsun.security.krb5.debug=true"`

`kafka-console-consumer --bootstrap-server <Broker1 IP>:9093,<Broker2 IP>:9093 --topic tst_gmc_doh_mca_db2_cdc_mbs_mist --consumer.config /home/luoshi/uat.client.properties --from-beginning`

The required keystore might be stored here in Cloudera:
/opt/cloudera/security/pki/zldhadnf01.central.health.jks
/usr/lib/jvm/jre/lib/security/jssecacerts
