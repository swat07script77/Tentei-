
{
    name = "BreakVelwwwssocity",
    desc = "breakvelocity | resets all velocity for 1 second",
    args = false,
    run = function(value)
        local char = player.Character
        if not char then return end

        local beenASecond = false
        local V3 = Vector3.new(0, 0, 0)

        task.delay(1, function()
            beenASecond = true
        end)

        while not beenASecond do
            for _, v in ipairs(char:GetDescendants()) do
                if v:IsA("BasePart") then
                    v.Velocity = V3
                    v.RotVelocity = V3
                end
            end
            task.wait()
        end
    end,
},
{
    name = "MaxSlopeAngle",
    desc = "maxslopeawwwngle (msa) | sets the max slope angle",
    args = true,
    run = function(value)
        local char = player.Character
        if not char then return end
        local hum = char:FindFirstChildWhichIsA("Humanoid")
        if not hum then return end

        local n = tonumber(value) or 89
        hum.MaxSlopeAngle = n
    end,
},
