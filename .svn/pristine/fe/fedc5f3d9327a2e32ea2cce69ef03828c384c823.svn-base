package ec.std.kurento;

import org.kurento.client.MediaPipeline;
import org.kurento.client.PlayerEndpoint;
import org.kurento.client.WebRtcEndpoint;

public class UserSession {

    private WebRtcEndpoint webRtcEndpoint;
    private MediaPipeline mediaPipeline;
    private PlayerEndpoint playerEndpoint;
    private String id;

    public UserSession() {
    }

    public UserSession(WebRtcEndpoint webRtcEndpoint, MediaPipeline mediaPipeline, PlayerEndpoint playerEndpoint) {
        this.webRtcEndpoint = webRtcEndpoint;
        this.mediaPipeline = mediaPipeline;
        this.playerEndpoint = playerEndpoint;
    }

    public WebRtcEndpoint getWebRtcEndpoint() {
        return webRtcEndpoint;
    }

    public void setWebRtcEndpoint(WebRtcEndpoint webRtcEndpoint) {
        this.webRtcEndpoint = webRtcEndpoint;
    }

    public MediaPipeline getMediaPipeline() {
        return mediaPipeline;
    }

    public void setMediaPipeline(MediaPipeline mediaPipeline) {
        this.mediaPipeline = mediaPipeline;
    }

    public PlayerEndpoint getPlayerEndpoint() {
        return playerEndpoint;
    }

    public void setPlayerEndpoint(PlayerEndpoint playerEndpoint) {
        this.playerEndpoint = playerEndpoint;
    }

    public String getId() {
        return id;
    }

    public void setId(String id) {
        this.id = id;
    }

    public void release() {
        this.playerEndpoint.stop();
        this.mediaPipeline.release();
    }

}
