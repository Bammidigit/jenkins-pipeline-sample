pipeline
{
    agent any
    stages
    {
        stage('scm checkout')
    {steps
    {sh 'echo code_is_downloading'}
  }
  
  
  stage('build the code')
  {steps
  {sh 'echo code_is_building'
   sh 'echo code is passed'}
      }

stage('deploy to dev en')
{steps
{sh 'echo deploying_aritifact_to_dev_ev'
}
}

stage ('Approve QA deployment')

{steps {input 'Please_approve_QA_deployment'}}

stage('deploy to QA en')
{steps
{sh 'echo deploying_aritifact_to_QA_ev'
}
}

    }
}
