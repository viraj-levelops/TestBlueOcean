pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build'
        script {
            Random rnd = new Random()
            def n = rnd.nextInt(10)
            println(n)
            println(n.getClass())

            for(int i=0; i< 1000000; i++) {
                n = rnd.nextInt(10)
                println(n)
                println(n.getClass())
            }

            def d = 10
            println(d.getClass())

            sleep(n)
            if(n % d == 0){
              error("Build Failed")
            }
        }
      }
    }

    stage('Unit Tests') {
      steps {
        echo 'Unit Tests'
        script {
        Random rnd = new Random()
        def n = rnd.nextInt(10)
        println(n)
        println(n.getClass())

        def d = 10
        println(d.getClass())

        sleep(n)
        if(n % d == 0){
          error("Unit Tests Failed")
        }
        }
      }
    }

    stage('Package') {
      steps {
        echo 'Package'
        script {
        Random rnd = new Random()
        def n = rnd.nextInt(10)
        println(n)
        println(n.getClass())

        def d = 10
        println(d.getClass())

        sleep(n)
        if(n % d == 0){
          error("Package Failed")
        }
        }
      }
    }

    stage('Deploy Stg1') {
      parallel {
        stage('Deploy Stg1') {
          steps {
            echo 'Deploy Stg1'
            script {
            Random rnd = new Random()
            def n = rnd.nextInt(10)
            println(n)
            println(n.getClass())

            def d = 10
            println(d.getClass())

            sleep(n)
            if(n % d == 0){
              error("Deploy Stg1 Failed")
            }
            }
          }
        }

        stage('Deploy Stg2') {
          steps {
            echo 'Deploy Stg2'
            script {
            Random rnd = new Random()
            def n = rnd.nextInt(10)
            println(n)
            println(n.getClass())

            def d = 10
            println(d.getClass())

            sleep(n)
            if(n % d == 0){
              error("Deploy Stg2 Failed")
            }
            }
          }
        }

        stage('Deploy Stg3') {
          steps {
            echo 'Deploy Stg3'
            script {
            Random rnd = new Random()
            def n = rnd.nextInt(10)
            println(n)
            println(n.getClass())

            def d = 10
            println(d.getClass())

            sleep(n)
            if(n % d == 0){
              error("Deploy Stg3 Failed")
            }
            }
          }
        }

      }
    }

    stage('Deploy Prod') {
      steps {
        echo 'Deploy Prod'
        script {
        Random rnd = new Random()
        def n = rnd.nextInt(10)
        println(n)
        println(n.getClass())

        def d = 10
        println(d.getClass())

        sleep(n)
        if(n % d == 0){
          error("Deploy Prod Failed")
        }
        }
      }
    }

  }
}