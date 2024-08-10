# Cloud Speech API 3 Ways: Challenge Lab 

export ZONE=$(gcloud compute instances list lab-vm --format 'csv[no-heading](zone)')
gcloud compute ssh lab-vm --project=$DEVSHELL_PROJECT_ID --zone=$ZONE --quiet

export API_KEY=""
export task_2_file_name=""
export task_3_request_file=""
export task_3_response_file=""
export task_4_sentence=""
export task_4_file=""
export task_5_sentence=""
export task_5_file=""

curl -LO raw.githubusercontent.com/dev-abhiig/dev-abhiig-ARC132/main/dev-abhiig-ARC132.sh

sudo chmod +x dev-abhiig-ARC132.sh

./dev-abhiig-ARC132.sh
