### Audio-Visual Event Localization in Unconstrained Videos: https://arxiv.org/abs/1803.08842  

* Audio-Visual Event is an event that is both visible and audible in a video segment
* Task is event localization. Given a video sequence of T overlapping segments each with an audio and video content, the task is to predict the event label for all the segments
* Supervised tasks are event localization in audio space alone, video space alone and cross modality localization (Given audio/visual track, predict the localization of the event in visual/audio track)
* Weakly supervised task is to predict the segment level labels during testing when the model is trained with only the video level event tag

#### Methodology for Supervised Task


