#!groovy
@Library('developWorkFlow')
import groovy.json.JsonSlurper
import org.codehaus.groovy.util.StringUtil
import org.yaml.snakeyaml.*
import org.yaml.snakeyaml.constructor.*
import groovy.transform.*
import com.td.devops.*

properties([disableConcurrentBuilds(), pipelineTriggers([])])

node('agent') {
    checkout scm
    def scmUrl = scm.getUserRemoteConfigs()[0].getUrl()
    env.scmUrl=scmUrl
