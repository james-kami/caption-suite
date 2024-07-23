1. first add soda by git submodule update --init --recursive
2. make sure the video is standarized using the .sh script.
3. add videos to the video folder
3. create a folder for model with .pth and info.json
4. create output folder

video_folder=visualization/videos
output_folder=visualization/output
pdvc_model_path=save/custom/model-best.pth
output_language=en
bash test_and_visualize.sh $video_folder $output_folder $pdvc_model_path $output_language

video_folder=visualization/videos
output_folder=visualization/custom_out
pdvc_model_path=save/custom/model-best.pth
output_language=en
bash test_and_visualize.sh $video_folder $output_folder $pdvc_model_path $output_language

video_folder=visualization/videos
output_folder=visualization/anet_out
pdvc_model_path=save/anet/model-best.pth
output_language=en
bash test_and_visualize.sh $video_folder $output_folder $pdvc_model_path $output_language
